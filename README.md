# proyecto2-3

Huggingface Api.

Proyecto 2 : implemente múltiples modelos, utilizando el api cree una clase que le permite iterar de un modelo a otro, en el readme detalla con un diagrama de flujo como estas usando los modelos y da un ejemplo del resultado.

## Descripción

Este proyecto utiliza la API de Hugging Face para implementar múltiples modelos, como un modelo LLM (Generador de texto) y un modelo de Resumen de texto. La API permite pasar un texto a través del modelo LLM para generar más texto y luego resumir el texto generado con el modelo de resumen.

La clase ModelSwitcher maneja la iteración entre ambos modelos, permitiendo que el texto sea primero procesado por el modelo LLM y luego resumido.

## Diagrama de flujo

![Proyecto_3 drawio](https://github.com/user-attachments/assets/0b2b83c9-4e2d-47ff-adf3-a33a24891320)

## Requisitos.

Para ejecutar este proyecto, el usuario necesitará:

  1. Python 3.7 o superior
  2. FastAPI.
  3. Hugging Face transformers.
  4. Uvicorn para correr el servidor.

     Puedes instalar las dependencias ejecutando:

     ```bash
     pip install fastapi uvicorn transformers

## Estructura del proyecto.

El proyecto tiene los siguientes archivos principales:

   1. app2.py: El servidor FastAPI que implementa la lógica de los modelos y las rutas de la API.
   2. README.md: Este archivo, que contiene la documentación del proyecto.

## Estructura del proyecto.
### API Endpoints.
#### GET.
Descripción: Este endpoint te da la bienvenida a la API.
### POST /generate_and_summarize/
Descripción: Este endpoint recibe un texto, lo procesa primero con el modelo de generación de texto (LLM), luego resume el texto generado.







