# Proyecto 3:

## Instrucciones del proyecto:

Instalación, configuración, crear y add (añadir) embedings, realizar consultas y usar condiciones y filtros avanzados en las consultas.

Crea un notebook en python (Python Colab) que permita realizar las operaciones de un CRUD, el readme debe contener:

1. **Explicar cada uno de los métodos de consulta en el CRUD**
2. **Explicar como configurar la  base de datos vectorial**
3. **Explicar el funcionamiento de los embedding y si configuracion**
4. **Debe contener imagenes de uso y ejemplos**

## Parte 1: Explicar cada uno de los métodos de consulta en el CRUD:

### Explicación:

CRUD: Es una sigla o acrónimo en inglés de las 4 operaciones de crear y gestionar datos que se hace en cualquier motor de base de datos como: Postgres, Microsoft SQL, entre otros, que cada una de las letras significa lo siguiente: La C significa CREATE o CREAR, la R significa OBTENER o LEER, la U significa UPDATE o ACTUALIZAR o MODIFICAR y por último la D significa DELETE o BORRAR o ELIMINAR. 

Objetivos: 

1. **Sirve para comprobar si efectivamente en una tabla específica de una base de datos se hizo cualquiera de las 4 operaciones mencionadas anteriormente, por ejemplo en Postman pongo GET http://localhost:3000/usuarios y me muestra todos los usuarios con todos sus atributos que existen en esa tabla de base de datos.**
2. **Las 4 operaciones manejan todos los datos de una aplicación que tiene el software.**

C (Create): Es una operación que crea un dato en una tabla específica, como ejemplo un usuario con los atributos por ejemplo (Nombre, Edad, Año de nacimiento, entre otros).

R (Read o Get): Es una operación que lee u obtiene todos los datos o un dato de una tabla específica.

U (Update o Actualizar): Es una operación que actualiza un dato específico de la tabla, por ejemplo ingresado un id de un objeto específico, ingresa los nuevos datos de un usuario y los actualiza.

D (Delete o Eliminar): Es una operación que elimina un dato específico de la tabla, por ejemplo ingresando un id de un objeto específico, posteriormente me sale un mensaje: "SE HA ELIMINADO CORRECTAMENTE DE LA BASE DE DATOS", el usuario comprueba en la base de datos y efectivamente se elimino.

## Parte 2: Explicar como configurar la  base de datos vectorial:

## Requisitos para la Ejecución

### Dependencias

1. **Python 3.8 a 3.10 independiente del sistema operativo que tenga el usuario como: Windows, Linux o Mac.**
2. **Visual studio instalado independiente del sistema operativo que tenga el usuario como: Windows, Linux o Mac.**
3. **Instalar el siguiente comando:**

    ``` bash
   pip install faiss-cpu transformers numpy scikit-learn torch matplotlib



Pasos:



## Explicar el funcionamiento de los embedding y si configuracion:

### ¿Qué son los embeddings?:

Los embeddings son una técnica de NLP (Natural Language Processing) que transforma el lenguaje humano en vectores matemáticos, por lo que sirve demasiado en la inteligencia artificial para los siguientes modelos como: Análisis de sentimientos, la clasificación del texto y la traducción automática.

## Parte 4: Debe contener imagenes de uso y ejemplos:

### Explicación:

Se mostrará ejemplos cuando el usuario va a usar la aplicación.

Pasos para que funcione el 100%.

#### Pasos:

1. **Primer lugar tiene que asegurar que tenga las siguientes dependencias como Python versión 3.8 mínimo y Visual Studio code independiente del sistema operativo que tenga en su ordenador.**
2. **Segundo lugar, tiene que clonar el proyecto en el computador que tenga con el siguiente comando:**

   ``` bash
   pip install faiss-cpu transformers numpy scikit-learn torch matplotlib











