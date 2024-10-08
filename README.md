# Lexicurium

## Descripción

Este proyecto tiene como objetivo crear un modelo de transcripción de audio utilizando Whisper AI, dockerizar el modelo y un script que cuenta palabras y letras, y automatizar la ejecución con un archivo `Makefile`.

## MVP:

### 1) [Levantar un modelo de Whisper AI en local](https://github.com/openai/whisper)
- El primer paso consiste en implementar y ejecutar localmente el modelo de Whisper AI utilizando Python y la biblioteca `whisper` de OpenAI.
- Además, dockerizaremos este modelo junto con el script que utilice `whisper` y un script adicional para contar palabras y letras.

### 2) Dockerizar Whisper AI y el script de Python
- Se creará un archivo `Dockerfile` para construir una imagen Docker que contenga:
  - El modelo Whisper AI.
  - Un script de Python para contar palabras o letras de una transcripción de audio.
  - Las dependencias necesarias definidas en un `requirements.txt`.

### 3) Crear un script para contar palabras y/o letras
- Se implementará un script en NodeJS que pueda contar palabras y/o letras de un texto proporcionado.
- Este script será ejecutado automáticamente después de la transcripción del audio mediante Whisper AI o de manera independiente.

### 4) Crear un Makefile
- Se añadirá un `Makefile` que incluya comandos para:
  - **Instalar** las dependencias del proyecto.
  - **Construir** la imagen de Docker.
  - **Ejecutar** el modelo Whisper AI y contar palabras/letras.
  - **Limpiar** archivos temporales o contenedores en desuso.
