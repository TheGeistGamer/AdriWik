# Glosario de Términos

## Docker

Docker es una herramienta diseñada para facilitar la creación, implementación y ejecución de aplicaciones mediante el uso de contenedores.

## Container/Contenedor

Es una instancia de una imagen ejecutándose en un ambiente aislado.

## Imagen de contenedor

Es un archivo construido por capas, que contiene todas las dependencias para ejecutarse, tal como: las dependencias, configuraciones, scripts, archivos binarios, etc.

## Dockerizar una aplicacón

Proceso de tomar un código fuente y generar una imagen lista para mostar y correla en una contenedor.

## DockerFile

Un archivo de texto con instrucciones necesarias para crear una imagen. Se peude ver como un blueprint o plano para su contrucción.

## .dockerignore

Similar al .gitignore, el .dockerignore especifica todo lo que hay que ignorar en un proceso de contrucción (build)

## docker-compose.yml

Archivo para definir los servidores y con un solo comando en lugar de definir todo directamente en la consola.

## Volumes

Proporcionan la capacidad de conectar rutas específicas del sistema de archivos del contenedor a la máquina host.

Si se monta un directorio en el contenedor, los cambios en ese directorio también se ven en la máquina host.

## Alpine - Linux

Alpine Linux es una distribución de Linux ligera y orientada a la seguridad basada en musl libc y busybox

## Nginx

Es un servidor web que también se puede utlizar como proxy inverso, blanaceador de carga, proxy de correo y caché HTTP. El software fue creado por Igor Sysoev y lanzado al público en 2004. Nginx es un software gratuito y de código abierto.

## Container Orchestration

La orquestación de contenedores es la automatización de gran parte del esfuerzo operativo requerido para ejecutar cargas de trabajo y servicios en contendedores.
Ejemplo de herramientas de orquestación son Kubernetes, Swarm, Nomad y ECS.

## Docker Layers

Las capas son el resultado de la forma en que se contruyen las imágenes de Docker. Cada paso en un Dockerfile crea una nueva **capa** que es esencialmente una diferencia de los cambios en el sistema de archivos desde el último paso.

## Snyk

Es una plataforma de seguridad para desarrolladores para proteger el código, las dependencias, los contenedores y la infraestructura com código.

## Registry

Es una aplicación del lado del servidor altamente escalable y sin estado que almacena y le permite distribuir imágenes de DOcker.

## Docker Deamon

Es el servicio en segundo plano que se ejecuta en el host que administra la creación, ejecución y distribución de contenedores Docker.
