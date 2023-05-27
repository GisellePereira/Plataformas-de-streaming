 ## **Proyecto_Individual**
>Giselle Pereira Nuñez

![Netflix-Amazon-Prime-Hulu-Disney-Plus-Logos](https://user-images.githubusercontent.com/108558805/220166602-27bce753-813d-4aec-af26-77c5e89cb28a.jpg)


:clipboard: **TEMÁTICA:**

Start-up que provee servicios de agregación de plataformas de streaming.
 
Como Data Scientist crearé un  modelo de ML que soluciona un problema de negocio: **un sistema de recomendación!**

Los datos se encuentran sin transformar, no hay procesos automatizados para la actualización de nuevas películas o series, entre otras cosas.

:round_pushpin: Asumiendo el rol completo de un Data Scientist :

Comienzo haciendo un trabajo de Data Engineer, donde se extrageron los datos de un almacenamiento en la nube, para transformarlos según lo necesitado.

Luego, un trabajo de Data Analytics, para realizar un EDA simple para obtener conocimiento básico y valioso de los datos.

Finalmente, modelando los datos y utilizando técnicas de aprendizaje automático, para crear un sistema de recomendación de ¡Peliculas y series!. 

:raised_hands: Manos a la obra :raised_hands:

-------------------------------------------------------------------------------------

**MENU:**

:heavy_check_mark: Carpeta 'API' - se encuentran todos los recursos necesarios para la API de consultas:
    
   - Spacefile: en este archivo se utiliza para configurar y definir los microservicios o funciones individuales dentro de la apicación
   - archivo1.parquet: datos almacenados en formato parquet(optimo para el procesamiento y análisis eficiente de grandes volúmenes de datos), utilizados pata la entrada en la API.
   - main.py: es el archivo principal de la API, construida con el lenguaje python en forma de **pipeline**, contiene el código fuente que define las rutas y funcionalidades de la API.
   - requirements.txt: este archivo de texto contiene una lista de paquetes y versiones requeridas para que la API funcione correctamente.

:heavy_check_mark: Carpeta 'Datasets_iniciales' - se encuentran en esta carpeta los datos iniciales, sin ninguna transformación:

   - amazon_prime_titles.csv: datos crudos de peliculas y series de la plataforma Amazon.
   - disney_plus_titles.csv: datos crudos de peliculas y series de la plataforma Disney Plus.
   - hulu_titles.csv: datos crudos de peliculas y series de la plataforma Hulu.
   - netflix_titles-csv: datos crudos de peliculas y series de la plataforma Netflix.

:heavy_check_mark: Carpeta 'Datasets_resultantes' - se encuentran en esta carpeta los datos resultantes del ETL (en formatos csv y parquet)y del ML (en formato parquet):

   - archivo.csv: datos resultantes de ETL en formato csv.
   - archivo1.parquet: datos resultantes de ETL en formato parquet.
   - ml.parquet: resultado del modelado de datos, para utilizarlos en el aprendizaje automático (ML)
    
:heavy_check_mark: Carpeta 'ETL_EDA' - dentro de esta carpeta se encuentran los archivos donde se realizaron el ETL y EDA (los dos en formato .ipynb):

   - ETL.ipynb: en este archivo se encuentra la extracción, transformación y limpieza de los datos crudos.
   - EDA.ipynb: en este archivo se encuentra una exploración de los datos.

:heavy_check_mark: Carpeta 'Informes' - en este carpeta se encuentran los informes del ETL y EDA:

   - Informe_ETL.pdf: en este informe se especifican los pasos realizados en el ETL, se explica el ¿Por qué? ¿Para qué? y su importancia (su formato es PDF).
   - Informe_EDA.pdf: en este informe se especifican los pasos realizados en el EDA, se explica el ¿Por qué? ¿Para qué? y su importancia (su formato es PDF).

:heavy_check_mark: Carpeta 'ML_funciones' - dentro de esta carpeta se encuentran las funciones realizadas para la API, y el machine learning:

   - Funciones_API.ipynb: en formato .ipynb, se encuentran las funciones que luego se utilizaron en el archivo principal "main.py". Y al final del archivo se encuenta la eliminación de los campos no utilizados.
   - ML.ipynb: en formato .ipynb, se encuentra el modelado de los datos, para luego utilizarlos en el aprendizaje automático donde se **predice si a un nuevo usuario le gustará o no una película o serie** teniengo en cuenta 

:heavy_check_mark: Carpeta '_ pycache' - esta carpera es creada automáticamente cuando se ejecuta el código de creación de la API, esta contiene archivos caché generados por el interprete para mejorar el rendimiento:

   - main.cpython-39.pyc: este archivo con la extención .pyc (archivo de código de bytes), es específco de la versión de python, no se modifican manualmente.

:heavy_check_mark: Archivo 'Netflix-Amazon-Prime-Hulu-Disney-Plus-Logos.jpg' - es la imagen que se encuentra al comienzo del readme.

:heavy_check_mark: Archivo 'README.md' - en este readme encontrará especificaciones de todo el proyecto.

-------------------------------------------------------------------------------------

**FUNCIONES QUE COMPONEN LA API Y EL LINK**
- Película con mayor duración,
     - Filtros opcionales: AÑO, PLATAFORMA Y TIPO DE DURACIÓN. 
     - Nombre de la función: get_max_duration(year, platform, duration_type)
- Cantidad de películas por plataforma teniendo en cuenta,
     -  Filtros no opcionsles: PLATAFORMA, PUNTAJE Y AÑO
     -  Nombre de la función: get_score_count(platform, scored, year))
- Cantidad de películas por plataforma teniendo en cuenta,
     - Filtro no opcional: PLATAFORMA.
     - Nombre de la función: get_count_platform(platform)
- Actor que más se repite según,
     - Filtros no opcionales: PLATAFORMA Y AÑO.
     - Nombre de la función: get_actor(platform, year)



:warning: **Sintaxis a tener en cuenta al escribir una consulta en los filtros de texto:** :warning:

:red_circle: Todo debe estar escrito en minúsculas.

:red_circle: Las plataformas admitidas: amazon, disney_plus, hulu y netflix.

:red_circle: En los filtros de tipo de duración colocar: min o season.


:link: En este [link](https://proyecto-1-l2915949.deta.app/docs) podras ingresar y consultar las funciones. Cliqueando en las 'flechas' de cada funsión, luego la opción 'Try it out', colocar los filtros y finalmente, cliquear botón 'Execute'.


**Relizarle solicitudes al servidor web de la API:**
- URL del servidor web: [https://proyecto-1-l2915949.deta.app/](https://proyecto-1-l2915949.deta.app/)
    - Si a esta URL se le agrega:
    
        :small_blue_diamond: get_max_duration(year, platform, duration_type) 
        
        :small_blue_diamond: get_score_count(platform, scored, year)
        
        :small_blue_diamond: get_count_platform(platform)
        
        :small_blue_diamond: get_actor(platform, year)
        
       **Devolverá una respuesta**
    
 - **Ejemplos:**
 
:link: [https://proyecto-1-l2915949.deta.app/get_max_duration](https://proyecto-1-l2915949.deta.app/get_max_duration)

:link: [https://proyecto-1-l2915949.deta.app/get_max_duration?year=2000&platform=amazon&duration_type=min](https://proyecto-1-l2915949.deta.app/get_max_duration?year=2000&platform=amazon&duration_type=min)

:link: [https://proyecto-1-l2915949.deta.app/get_score_count?platform=netflix&scored=3&year=2001](https://proyecto-1-l2915949.deta.app/get_score_count?platform=netflix&scored=3&year=2001)

:link: [https://proyecto-1-l2915949.deta.app/get_count_platform?platform=hulu](https://proyecto-1-l2915949.deta.app/get_count_platform?platform=hulu)

:link: [https://proyecto-1-l2915949.deta.app/get_actor?platform=disney_plus&year=2012](https://proyecto-1-l2915949.deta.app/get_actor?platform=disney_plus&year=2012)


Descargar la app aqui: https://deta.space/discovery/r/cwp6zzbnkbpl6yml
+ Space Deta
>Usuario: gipereira2023

>Nombre de la app: PROYECTO

-------------------------------------------------------------------------------------

:wrench: **EN ESTE PROTECTO SE UTILIZARON LAS SIGUIENTES HERRAMIENTAS**

- Python.
- Visual studio code.
- Librería pandas.
- Librería numpy.
- Librería seaborn.
- Librería matplotlib.
- Librería datetime.
- Librería scikit-learn.
- Librería surprise.
- Librería fastparquet.
- FastApi.
- Uvicorn (servidor web).
- Space Deta (plataforma online y gratuita)

Gracias por la visita :smile: :bangbang:

**MI CONTACTO:**

:fire: [Gmail](mailto:giseepereira2017@gmail.com)

:fire: [LinkedIn](https://www.linkedin.com/in/giselle-pereira-nu%C3%B1ez-011330168/)




