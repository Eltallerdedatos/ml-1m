# MovieLens 1M Dataset 📊🎬

Bienvenido al repositorio del **MovieLens 1M Dataset**. Este conjunto de datos contiene más de **1 millón de valoraciones de películas** realizadas por usuarios. Es ideal para tareas de **recomendación de películas** y análisis de datos.

## Archivos del Dataset 📁
- **`movies.dat`**: Información sobre las películas, incluyendo su **título** y **género**. 🎥
- **`users.dat`**: Información sobre los usuarios, como **género**, **edad**, **ocupación** y **código postal**. 👤
- **`ratings.dat`**: Las **valoraciones** realizadas por los usuarios a las películas. ⭐

Este dataset es ampliamente utilizado en el área de **sistemas de recomendación** y **aprendizaje automático**. ¡Explora los datos y comienza a construir tu modelo de recomendación! 🤖

---

## Cómo usar el dataset 🔧

1. **Descargar los archivos**: Puedes descargar los archivos directamente desde este repositorio o utilizarlos en tu proyecto de Python o cualquier otro entorno de análisis de datos.
2. **Cargar los datos**: Utiliza bibliotecas como **Pandas** en Python para cargar los datos y empezar a analizarlos.
   
   Ejemplo de código para cargar los datos en Python:
   ```python
   import pandas as pd

   # Cargar el dataset de películas
   movies = pd.read_csv('movies.dat', sep='::', header=None, names=['movie_id', 'title', 'genre'], engine='python')

   # Cargar el dataset de usuarios
   users = pd.read_csv('users.dat', sep='::', header=None, names=['user_id', 'gender', 'age', 'occupation', 'zipcode'], engine='python')

   # Cargar el dataset de valoraciones
   ratings = pd.read_csv('ratings.dat', sep='::', header=None, names=['user_id', 'movie_id', 'rating', 'timestamp'], engine='python')

   # Ver los primeros registros
   print(movies.head())
   print(users.head())
   print(ratings.head())

   


