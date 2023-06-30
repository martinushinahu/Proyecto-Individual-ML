# Proyecto-Individual-ML
Desarrollado por Martin Ushinahua Quinteros

# API de Recomendación de Películas
Esta API de Recomendación de Películas es un proyecto que tiene como objetivo proporcionar recomendaciones personalizadas de películas a los usuarios. Utiliza técnicas de Procesamiento del Lenguaje Natural (NLP) y algoritmos de similitud para encontrar películas similares a una película de entrada dada por el usuario

## 🌟Proceso de ETL (Extracción, Transformación y Carga)
El proceso de ETL se realizó para preparar los datos necesarios para la API de recomendación de películas. A continuación, se describe el proceso paso a paso:

1. Extracción: Se obtuvieron dos conjuntos de datos para este proyecto. El primer conjunto de datos es una base de datos de películas que contiene información sobre títulos, géneros y otras características de las películas. El segundo conjunto de datos es un archivo CSV que contiene críticas y puntuaciones de películas realizadas por usuarios.
los datasets brindados:
- movies_dataset.csv
- credits.csv
  
📚 [Fuente de Datasets](https://drive.google.com/drive/folders/1d25XsXOWwp1d_Dh5Qwqx1GNu5DD1YV21?usp=drive_link)
  
2. Transformación: Se llevaron a cabo varias transformaciones en los datos extraídos para prepararlos para el modelo de recomendación. Esto incluyó la limpieza y preprocesamiento de los textos de las críticas, la combinación de los conjuntos de datos de películas y críticas en uno solo, y la generación de una matriz de características para calcular la similitud entre películas.
3. Carga: Los datos transformados se almacenaron en un formato adecuado para su posterior uso en la API de recomendación de películas.

  ➡️ [Aquí en el proceso de ETL de los datos](https://github.com/martinushinahu/Proyecto-Individual-ML/blob/main/ETL/limpieza_datos.ipynb)


## 🎯 Objetivo y propósito
El objetivo principal de esta API es proporcionar a los usuarios recomendaciones personalizadas de películas basadas en sus preferencias y en películas similares a las que les gustan. Algunos de los beneficios y propósitos de esta API son:

- Ayudar a los usuarios a descubrir nuevas películas que les puedan interesar, basadas en sus gustos y preferencias anteriores.
- Proporcionar una experiencia de recomendación personalizada y adaptada a cada usuario.
- Permitir a los usuarios explorar películas similares a las que ya han visto y disfrutado.
- Servir como una herramienta útil para desarrolladores de aplicaciones, sitios web o servicios relacionados con películas, que deseen incorporar recomendaciones de películas en sus proyectos.

## 📖Despliegue
La API de Recomendación de Películas se ha desplegado en la plataforma Render, lo que permite un acceso fácil y rápido a la funcionalidad de recomendación de películas. Los usuarios pueden enviar consultas a la API utilizando los endpoints correspondientes y recibir recomendaciones de películas en respuesta.

➡️ [Proceso de despliegue del desarrollo de la Api](https://github.com/martinushinahu/deploy_api)

## 🧩 Machine Learning
El proceso esta basado en el enfoque de filtrado colaborativo, ya que se calcula la similitud entre películas y se recomiendan las más similares.

1. Preprocesamiento de datos: Se utiliza la biblioteca TfidfVectorizer para convertir el texto de la columna 'overview' en una representación numérica utilizando la técnica de TF-IDF (Term Frequency-Inverse Document Frequency). Esto ayuda a capturar la importancia relativa de las palabras en el contexto del conjunto de películas.

2. Cálculo de similitud: Se calcula la similitud coseno entre las películas utilizando la matriz de características TF-IDF. La similitud coseno es una medida común utilizada en sistemas de recomendación para determinar la similitud entre dos elementos en función de sus características.

3. Función de recomendación: La función obtener_recomendaciones toma como entrada el título de una película y utiliza la similitud coseno para encontrar las películas más similares. Ordena las películas según los puntajes de similitud y devuelve las primeras 5 películas recomendadas.

➡️ [Proceso de Machine Learning ](https://github.com/martinushinahu/Proyecto-Individual-ML/blob/main/ML/machine_learnig.ipynb)

## 🖥️Uso de la API

Se agrego una Interfaz para poder hacer uso sencilo de la API
➡️ [La API está disponible](https://api-recomendacion-de-peliculas.onrender.com)


## 👥Contribuciones y mejoras
Este proyecto de API de Recomendación de Películas está en constante desarrollo y se pueden realizar contribuciones y mejoras adicionales. Si deseas colaborar o tienes ideas para mejorar la funcionalidad de la API, ¡no dudes en contribuir al proyecto!

## 📜Licencia
Este proyecto se distribuye bajo la Licencia MIT. Para obtener más información, consulta el archivo LICENSE en este repositorio.


¡Gracias por utilizar la API de Recomendación de Películas! Esperamos que encuentres útil esta herramienta para descubrir nuevas películas y disfrutar de una experiencia de recomendación personalizada. Si tienes alguna pregunta o necesitas ayuda, no dudes en contactarnos. ¡Disfruta explorando películas!
