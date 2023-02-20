                                                                  Proyecto_Individual01
Giselle Pereira Nuñez



Temática
El Rol consiste en Data Scientist que trabaja en una start-up que provee servicios de agregación de plataformas de streaming. Voy a crear mi primer modelo de ML que soluciona un problema de negocio: un sistema de recomendación que aún no ha sido puesto en marcha!

Voy a los datos y me doy cuenta que la madurez de los mismos es poca: Datos sin transformar, no hay procesos automatizados para la actualización de nuevas películas o series, entre otras cosas😩.

Empiezo desde 0, haciendo un trabajo de Data Engineer y comenzar con mi primer modelo de ML❗. 

Manos a la obra 💪


MENU: 

Carpeta Datasets_iniciales - las bases de datos que recibí para trabajar.
Carpeta pycache - carpeta necesaria para el funcionamiento de la API.
Carpeta API - dentro de encuentan todo los recursos necesarios para la API de consultas.
Funciones_API.ipynb - notebook con pruebas de las funciones.
ETL.ipynb - paso a paso del ETL.
EDA.ipynb - archivo de analisis de datos.
ML.ipynb - acrchivo de modelo de Sistema de Recomendación.
README - Instrucciones de uso.
ml.parquet - archivo parquet utilizado para el modelo de ML.


Funciones que componen la API y Link:
- Película con mayor duración con filtros opcionales de AÑO, PLATAFORMA Y TIPO DE DURACIÓN. 
- Cantidad de películas por plataforma con un puntaje mayor a XX en determinado año.
- Cantidad de películas por plataforma con filtro de PLATAFORMA.
- Actor que más se repite según plataforma y año. 


En este link podras ingresar y consultar las funciones: https://proyecto-1-l2915949.deta.app/
- get_max_duration(year, platform, duration_type) opcional parametros
- get_score_count(platform, scored, year))
- get_count_platform(platform)
- get_actor(platform, year)

Ejemplo de ponerle opciones: "app/get_max_duration/OPCION_AÑO_OPCION_PLATAFORMA_OPCION_TIPODURACION"

Tambien puedes agregarle /docs, te sera mas amistoso! - https://proyecto-1-l2915949.deta.app/docs

Sintaxis a tener en cuenta al escribir una consulta: ⚠️
- Todo debe estar escrito en minúsculas.
- Las plataformas que admite son: amazon, disney_plus, hulu y netflix.

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
Cualquier cosa podes escribirme a --> giseepereira2017@gmial.com


