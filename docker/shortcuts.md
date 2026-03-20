# Guia de atajos

## Commandos Básicos

### Descargar una imagen

```bash
docker pull IMAGE_NAME
docker pull IMAGE_NAME:TAG
docker pull postgres
docker pull postgress:15.1
```

### Correr un contenedor

```bash
docker container run IMAGE_NAME
docker container run -d -p 80:80 docker/getting-started
```

`-d:` **Corre la imagen desenlazada** de la consola donde se ejecutó el comando.
`-p 80:80:` **Mapea el puerto 80** de nuestra computadora con el puerto 80 del contenedor.
`docker/getting-started:` **imagen a usar**

### Puedes combinar banderas

```bash
docker container run -db 80:80 docker/getting-started
docker run -db 80:80 docker/getting-started
```

### Obtener ayuda de un comando

```bash
  docker `<comando>` --help
```

### Asignar un nombre al contendor

```bash
  docker container run --name myName docker/getting-started
```

### Mostrar un listado de todos los contenedores corriendo en el equipo

```bash
docker container ls
docker ps
```

### Mostrar todos los contenedores del equipo

```bash
docker container ls -a
docker ps -a
```

### Detener un contenedor y eliminarlo

```bash
docker container stop `<container-id>`
docker container rm `<container-id>`
```

### Iniciar un contenedor previamente creado

```bash
docker container start `<container-id>`
```

### Dentener el contenedor (o varios) y removerlos de forma forzada

```bash
docker container rm -f `<container-id> o <ID1 ID2...>
```

`Container-id:` Pueden ser los primeros 3 dígitos

### Autenticarte en `docker.hub`

```bash
docker login -u `<Tu Usuario>`
```

O bien, puedes crear tokens de accesso específicos.

## Imágenes

### Construir y asignar un tag a la imagen

El objetivo del tag es que sea fácil de identificar y leer por humanos

```bash
docker build -t getting-started
```

`-t:` Asigna el tag name
`.:` Indica. a dónde buscar el archivo **DockerFile** en el directorio actual.

### Renombrar una imagen local

```bash
docker image tag SOURCE[:TAG] TARGET_IMAGE[:TAG]
docker tag IMAGE NEW_IMAGE
docker tag `<Tag Actual>` `<USUARIO>`/`<NUEVO NOMBRE>`

docker tag getting-started YOUR-USERNAME/getting-started
```

Este comando es comúm para desplegar imágenes en diferentes registros.

Si se olvida el número de versión o lo quieres colocar

```bash
docker image tag IMAGEN IMAGEN:2.0.0
```

## Limpieza de imágenes

### Listado de todas las imágenes

```bash
docker images
```

### Eliminar una imagen específica

```bash
docker image rm `<image_id>` o `<ID1 ID2 ID3 ...>`
docker rmi IMAGE
docker rmi getting-started
```

### Eliminar imágenees colgadas

```bash
docker image prune
```

### Borrar todas las imágenes no usadas

```bash
docker iamge prune -a
```

## Logs y examinar contenedores

### Mostrar logs de un contenedor

```bash
docker container logs `<container-id>`
docker container logs --follow CONTAINER
```

`--follow:` Seguir los nuevos logs mostrados

### Mostrar estadísticas y consumo de memoria

```bash
docker stats
```

### Iniciar un comando `shell` dentor del contenedor

```bash
docker exec -it CONTAINER EXECUTABLE
docker exce -it web bash
docker exce -it web /bin/sh
```

`-it:` Interactive Terminal
