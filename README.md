 Proyecto_Individual01
>Giselle Pereira Nuñez

![Netflix-Amazon-Prime-Hulu-Disney-Plus-Logos](https://user-images.githubusercontent.com/108558805/220166602-27bce753-813d-4aec-af26-77c5e89cb28a.jpg)


Temática: 

Soy un Data Scientist que trabaja en una start-up que provee servicios de agregación de plataformas de streaming. Voy a crear mi primer modelo de ML que soluciona un problema de negocio: un sistema de recomendación que aún no ha sido puesto en marcha!

Voy a los datos y me doy cuenta que la madurez de los mismos es poca: Datos sin transformar, no hay procesos automatizados para la actualización de nuevas películas o series, entre otras cosas😩.

Empiezo desde 0, haciendo un trabajo de Data Engineer y comenzar con mi primer modelo de ML❗. 

Manos a la obra 💪


MENU: 

- [x] Carpeta Datasets_iniciales - las bases de datos que recibí para trabajar.
- [x] Carpeta pycache - carpeta necesaria para el funcionamiento de la API.
- [x] Carpeta API - dentro de encuentan todo los recursos necesarios para la API de consultas.
- [x] Funciones_API.ipynb - notebook con pruebas de las funciones.
- [x] ETL.ipynb - paso a paso del ETL.
- [x] EDA.ipynb - archivo de analisis de datos.
- [x] ML.ipynb - acrchivo de modelo de Sistema de Recomendación.
- [x] README - Instrucciones de uso.
- [x] ml.parquet - archivo parquet utilizado para el modelo de ML.


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

Descargar la app aqui: https://deta.space/discovery/r/cwp6zzbnkbpl6yml

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
Cualquier cosa podes escribirme a --> giseepereira2017@gmial.com


