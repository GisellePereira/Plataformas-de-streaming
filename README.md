 ## **Proyecto_Individual**
>Giselle Pereira Nuñez

![Netflix-Amazon-Prime-Hulu-Disney-Plus-Logos](https://user-images.githubusercontent.com/108558805/220166602-27bce753-813d-4aec-af26-77c5e89cb28a.jpg)


:clipboard: Temática: 

Start-up que provee servicios de agregación de plataformas de streaming.
 
Como Data Scientist crearé un  modelo de ML que soluciona un problema de negocio: **un sistema de recomendación!**

Los datos se encuentran sin transformar, no hay procesos automatizados para la actualización de nuevas películas o series, entre otras cosas.

:round_pushpin: Asumiendo el rol completo de un Data Scientist :

Comienzo haciendo un trabajo de Data Engineer, donde se extrageron los datos de un almacenamiento en la nube, para transformarlos según lo necesitado.

Luego, un trabajo de Data Analytics, para realizar un EDA simple para obtener conocimiento básico y valioso de los datos.

Finalmente, modelando los datos y utilizando técnicas de aprendizaje automático, para crear un sistema de recomendación de ¡Peliculas y series!. 

:raised_hands: Manos a la obra :raised_hands:

MENU: 

:heavy_check_mark: Carpeta 'API' - se encuentran todos los recursos necesarios para la API de consultas:
    
   - Spacefile: en este archivo se utiliza para configurar y definir los microservicios o funciones individuales dentro de la apicación
   - archivo1.parquet: datos almacenados en formato parquet(optimo para el procesamiento y análisis eficiente de grandes volúmenes de datos), utilizados pata la entrada en la API.
   - main.py: es el archivo principal de la API, construida con el lenguaje python en forma de **pipeline**, contiene el código fuente que define las rutas y funcionalidades de la API.
   - requirements.txt: este archivo de texto contiene una lista de paquetes y versiones requeridas para que la API funcione correctamente.

:heavy_check_mark: Carpeta 'Codigo_Transformación_Exploración' - dentro de encuentan todo los recursos necesarios para la API de consultas.
    
:heavy_check_mark: Carpeta Datasets_iniciales - las bases de datos que recibí para trabajar.

:heavy_check_mark: Carpeta pycache - carpeta necesaria para el funcionamiento de la API.

:heavy_check_mark: Carpeta API - dentro de encuentan todo los recursos necesarios para la API de consultas.

:heavy_check_mark: Funciones_API.ipynb - notebook con pruebas de las funciones.

:heavy_check_mark: ETL.ipynb - paso a paso del ETL.

:heavy_check_mark: EDA.ipynb - archivo de analisis de datos.

:heavy_check_mark: ML.ipynb - acrchivo de modelo de Sistema de Recomendación.

:heavy_check_mark: README - Instrucciones de uso.

:heavy_check_mark: ml.parquet - archivo parquet utilizado para el modelo de ML.


Funciones que componen la API y Link:
- Película con mayor duración con filtros opcionales de AÑO, PLATAFORMA Y TIPO DE DURACIÓN. 
- Cantidad de películas por plataforma con un puntaje mayor a XX en determinado año.
- Cantidad de películas por plataforma con filtro de PLATAFORMA.
- Actor que más se repite según plataforma y año. 


En este link podras ingresar y consultar las funciones: [Link](https://proyecto-1-l2915949.deta.app/)
- get_max_duration(year, platform, duration_type) opcional parametros
- get_score_count(platform, scored, year))
- get_count_platform(platform)
- get_actor(platform, year)

Ejemplo de ponerle opciones: "app/get_max_duration/OPCION_AÑO_OPCION_PLATAFORMA_OPCION_TIPODURACION"

Tambien puedes agregarle /docs, te sera mas amistoso! - [Link](https://proyecto-1-l2915949.deta.app/docs)

Descargar la app aqui: https://deta.space/discovery/r/cwp6zzbnkbpl6yml
+ Space Deta
>Usuario: gipereira2023

>Nombre de la app: PROYECTO

Sintaxis a tener en cuenta al escribir una consulta: ⚠️
- Todo debe estar escrito en minúsculas.
- Las plataformas que admite son: amazon, disney_plus, hulu y netflix.
- En los campos que piden tipo de duración estan las opciones: min y season.

Use estas heramientas:
- Python.
- Librería Pandas.
- Librería Numpy.
- Librería scikit-learn.
- FastApi.
- Uvicorn.
- Space Deta (plataforma online y gratuita)
- Entre Otros!!

Gracias por la visita😏
Cualquier cosa podes escribirme a --> giseepereira2017@gmial.com :+1:


