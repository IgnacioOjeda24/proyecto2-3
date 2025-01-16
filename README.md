# Proyecto 3:

## Instrucciones del proyecto:

Instalación, configuración, crear y add (añadir) embedings, realizar consultas y usar condiciones y filtros avanzados en las consultas.

Crea un notebook en python (Python Colab) que permita realizar las operaciones de un CRUD, el readme debe contener:

1. **Explicar cada uno de los métodos de consulta en el CRUD**
2. **Explicar como configurar la  base de datos vectorial**
3. **Explicar el funcionamiento de los embedding y si configuracion**
4. **Debe contener imagenes de uso y ejemplos**

## Introducción del proyecto:

Este proyecto demuestra cómo implementar un sistema CRUD (Crear, Leer u Obtener, Actualizar o Modificar, Eliminar o Borrar cualquier dato, texto, información, entre otros) utilizando la biblioteca de python de base de datos vectores que se llama FAISS para trabajar en el proyecto. Aparte, se utiliza el modelo de lenguaje DistilBERT de la empresa estadounidense Hugging Face para generar embeddings de texto, realizar búsquedas por similitud y posteriormente gráficarlos.

## Parte 1: Explicar cada uno de los métodos de consulta en el CRUD:

### Explicación:

CRUD: Es una sigla o acrónimo en inglés de las 4 operaciones de crear y gestionar datos que se hace en cualquier motor de base de datos como: Postgres, Microsoft SQL, entre otros, que cada una de las letras significa lo siguiente: La C significa CREATE o CREAR, la R significa OBTENER o LEER, la U significa UPDATE o ACTUALIZAR o MODIFICAR y por último la D significa DELETE o BORRAR o ELIMINAR. 

Objetivos: 

1. **Sirve para comprobar si efectivamente en una tabla específica de una base de datos se hizo cualquiera de las 4 operaciones mencionadas anteriormente, por ejemplo en Postman pongo GET http://localhost:3000/usuarios y me muestra todos los usuarios con todos sus atributos que existen en esa tabla de base de datos.**
2. **Las 4 operaciones manejan todos los datos de una aplicación que tiene el software.**

C (Create): Es una operación que crea un dato en una tabla específica, como ejemplo un usuario con los atributos por ejemplo (Nombre, Edad, Año de nacimiento, entre otros).   En este caso se usa para añadir un texto en la base de datos vectoriales de python que se llama FAISS, los pasos a seguir son: Generar el embedding del texto utilizando el modelo de Hugging Face llamado distilbert/distilbert-base-uncased, almacena el texto en una lista de diccionarios de los textos que agregó el usuario e indexar el embedding en la base de datos vectoriales mencionada anteriormente. NOTA: La función que se ocupará en el proyecto es: create_document().

R (Read o Get): Es una operación que lee u obtiene todos los datos o un dato de una tabla específica de cualquier base de datos. NOTA: Se mostrará todos los datos que ingresó el usuario en el motor de la base de datos seleccionada por el programador. NOTA: La función que se usará es get_document().


U (Update o Actualizar): Es una operación que permite actualizar un dato específico de la tabla de la base de datos, por ejemplo ingresado un index de un objeto específico o que seleccione el usuario, ingresa su nuevo texto y sale que se ha actualizado correctamente. Los pasos a seguir son: Este proceso se trata de generar el nuevo embedding basado en el texto modificado, se cambia el texto como el embedding de las listas correspondientes de la base de datos FAISS. NOTA: La función que se usará es update_document().

D (Delete o Eliminar): Es una operación que elimina un dato específico de la tabla, por ejemplo ingresando un id de un objeto específico, posteriormente me sale un mensaje: "SE HA ELIMINADO CORRECTAMENTE DE LA BASE DE DATOS", el usuario comprueba en la base de datos y efectivamente se elimino. Los pasos para seguir son:El usuario ingresa al menú cuatro y su embedding asociados a la lista que existe y se modificará el índice FAISS sin el documento borrado.

## Parte 2: Explicar como configurar la  base de datos vectorial:

## Requisitos para la Ejecución

### Dependencias

1. **Python 3.8 a 3.10 independiente del sistema operativo que tenga el usuario como: Windows, Linux o Mac.**
2. **Visual studio instalado independiente del sistema operativo que tenga el usuario como: Windows, Linux o Mac.**
3. **Instalar el siguiente comando de instalar las librerías:**

   ##### Comando:

      ``` bash
      pip install faiss-cpu transformers numpy scikit-learn torch matplotlib

  ##### Ejemplo:

       ![Foto3](https://github.com/user-attachments/assets/92258a1e-881a-44a9-9460-64c794a1be16)

4. ** A las vez al tener las librerías instaladas de todo el proyecto, se tiene que configurar la base de datos en python, que esta vez se eligió FAISS, ya que es menor complejo y más sencillo.

5. **FAISS: Es una biblioteca o librería de python de código diseñado para la búsqueda y el almacenamiento rápido de similitudes y la agrupación de vectores densos. Este proyecto se usará parámetros como: Dimensión de los embeddings : 768 (salida de DistilBert) y tipo de índice (IndexFlatL2) que es la distancia euclidana plana.

6. **Configuración simple de la base de datos**

      Importar la librería.

         ![Foto8](https://github.com/user-attachments/assets/eb5f8f7b-3331-4d44-896a-8b03ac048071)

   

      Crear un índice:

         ![Foto9](https://github.com/user-attachments/assets/24bc1e74-2dee-41f9-bd7a-3de0e8d7a095)

      
     Agregar embeddings al índice.

         ![Foto10](https://github.com/user-attachments/assets/c7a92fef-c5f6-486d-93b2-07fdb47bf4a9)

## Parte 3:  Explicar el funcionamiento de los embedding y su configuracion:

### ¿Qué son los embeddings?:

Los embeddings son una técnica de NLP (Natural Language Processing) que transforma el lenguaje humano en vectores matemáticos, por lo que sirve demasiado en la inteligencia artificial para los siguientes modelos como: Análisis de sentimientos, la clasificación del texto y la traducción automática.

**Tokenización: Transforma texto en una secuencia de índices numéricos.**

![Foto11](https://github.com/user-attachments/assets/8ad2b182-5496-452d-9a24-faa89d0a8897)

**Cálculo de embedding: Usa el modelo para obtener la representación vectorial**

![Foto12](https://github.com/user-attachments/assets/d696b507-ac3f-4182-b004-a5cc46a31908)

**Configuración: El modelo DistilBERT se descarga de forma automática desde Hugging Face al inicializar.

![Foto13](https://github.com/user-attachments/assets/7d7e7716-3eb9-4ab8-a962-bf4af5f0199c)


## Parte 4: Debe contener imagenes de uso y ejemplos:

### Explicación:

Se mostrará ejemplos cuando el usuario va a usar la aplicación.

Pasos para que funcione el 100%.

#### Pasos:

1. **Primer lugar tiene que asegurar que tenga las siguientes dependencias como Python versión 3.8 mínimo y Visual Studio code independiente del sistema operativo que tenga en su ordenador.**
2. **Segundo lugar, tiene que clonar el proyecto en el computador que tenga con el siguiente comando:**

   ``` bash
   git clone https://github.com/IgnacioOjeda24/base-de-datos-vectorial.git

3. **Tercer lugar, posteriormente a clonarlo, el usuario que abrir una terminal en visual studio code, donde la pestaña de terminal**
4. **Cuarto lugar, al abrir la terminal tiene que ejecutar el siguiente comando, para crear el entorno virtual en visual studio code**

   ##### Comando:

     ``` bash
     python -m venv nombre_entorno_virtual

  ##### Ejemplo:

     ``` bash
     python -m venv ev

5. **Quinto lugar, a la vez que se haya creada el entorno virtual, el usuario tendrá que ejecutar el siguiente comando:**

   ##### Comando:

     ``` bash
     nombre_entorno_virtual\Scripts\activate

  ##### Ejemplo:

     ``` bash
     ev\Scripts\activate


6. **Sexto lugar, ahora hay que ejecutar los comandos para instalar las librerías de python como las que se muestran al continuación:**

    ![image](https://github.com/user-attachments/assets/d04af08b-01b5-4edf-a4b9-7f0f22ec3133)

7. **Séptimo lugar, a la vez que se haya instalado las librerías, se importa en el python colab:**

    ![image](https://github.com/user-attachments/assets/f0f98ac1-83dc-424a-ba86-0a7fad0f3f29)
   
8. **Octavo lugar, al ejecutar el proyecto se muestra la presentación del menú**

     **Foto 1**
       
     ![Capture001](https://github.com/user-attachments/assets/55d2de0c-f11f-4826-9bd6-79be55d53e46)

     **Foto 2**
     
     ![image](https://github.com/user-attachments/assets/5b9e9db0-ae3d-4fc7-81f4-ed2f4280785b)


9. **Noveno lugar, al seleccionar la opción 1: Se añade un documento cualquier nombre, pero en este caso ingresé con los nombres de las series de netflix en inglés como Wednesday (Merlina) y se agregó el documento correctamente**

    ![image](https://github.com/user-attachments/assets/3d16db34-cdda-4d81-b596-58d5a2cc961f)

10. **Décimo lugar, al seccionar la opción 2: Se obtiene todos los documentos que ingresó el usuario, en este caso los nombres de los títulos de las series de netflix en inglés.**
       
    ![image](https://github.com/user-attachments/assets/bb133ab9-c477-45f4-862d-0f82a8df60a5)

11. **Undécimo lugar, al seleccionar la opción 3: Se cambia el nombre del documento de un índex específico, que se seleccionó el 1 que pasará de Wednesday a Money Heist (Casa de papel)**

       **Foto a actualizar un índex específico que es el 1 y se hizo de manera satisfactoria**

       ![image](https://github.com/user-attachments/assets/171b9ee7-8362-4a48-8413-a6b605c3a069)

       **Foto que está actualizada la base de datos**

       ![image](https://github.com/user-attachments/assets/31253445-44bb-43c2-9426-895282ca352d)

12. **Duodécimo lugar, al seleccionar la opción 4: Se eliminar un índex específico y para comprobar se hace a través del menú 2**

      **Foto para eliminar el índex**

      ![image](https://github.com/user-attachments/assets/88c4dff2-696b-433f-81fb-fd9ad3510087)

      **Efectivamente se eliminó el documento de la serie de netflix: "House of Card"**

      ![image](https://github.com/user-attachments/assets/071ba578-41a6-4853-a4cd-bc447aab4357)

13. **Décimo tercero, al seccionar la opción 5, el usuario pone una palabra para poner la similitud y arrojan resultados entre 0 y 1**

      ![image](https://github.com/user-attachments/assets/a70e411b-d516-4963-998b-2dd3a54ddac2)

14 **Décimo cuarto lugar, al seleccionar la opción 6, sale el gráfico de 2D**

      ![WhatsApp Image 2025-01-15 at 10 23 19 PM](https://github.com/user-attachments/assets/f4fd4c1e-66f6-46d3-8b9c-5fae5da841e4)

      ![WhatsApp Image 2025-01-15 at 10 23 45 PM](https://github.com/user-attachments/assets/5c009f3f-c79e-461a-9174-99d2aba7b544)
  

15 **Décimo quinto lugar, al seleccionar la opción 7, se termina la ejecución del programa**

      ![F1](https://github.com/user-attachments/assets/f8823ee3-922f-4016-9402-0c926c82e734)




      





   

   











