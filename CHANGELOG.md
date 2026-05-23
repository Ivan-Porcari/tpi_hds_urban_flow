# Changelog

Todos los cambios notables del proyecto Urban Flow 
serán documentados en este archivo.
El formato está basado en 
[Keep a Changelog](https://keepachangelog.com).

## [0.1.0] - 2026-04-16

### Added
- Inicialización del repositorio git
- Configuración del archivo .gitignore
- Creación del archivo README.md
- Creación de la estructura de carpetas del proyecto


## [0.2.0] - 2026-04-23

### Added
- Incorporación delarchivo 'speeding_fines.csv' a la carpeta raw del proyecto
- Carga de dataset 'speeding_fines.csv' mediante pathlib.
- Analisis de tipo (dtypes) y  valores nulos (isnull().sum()).
- Creación de la rama ejercicio_2_3


## [0.3.0] - 2026-04-24

### Added
- Normalización de fechas con formato YYYY-MM-DD
- Normalización de horas a formato 24 HS 
- Normalización de Ubicaciones, se quitaron caracteres especiales y se pasaron a mayúsculas
- Normalización de patentes, se quitaron caracteres especiales y pasaron a mayúsculas.
- Se eliminaron las filas que tenían inconsistencia de datos que imposibilitaban las generación de la infracción
- Se buscaron outliers en las columnas numericas
- Se creo la columna exceso_velocidad_real y exceso_velocidad
- Se eliminaron las filas con patentes que no cometieron infracciones.
- Se generó un dataset limpio en la carpeta interim



## [0.3.1] - 2026-04-25

### Fixed
- Se corrigio el codigo para que los datos invalidos representados con 1932-01-01 y 00:00, queden en el dataset 
para su posterior uso.


## [0.3.0] - 2026-04-25

### Added
- Ejercicio 04: clase FineAnalyzer con encapsulamiento y 5 metodos de analisis
- Punto 05: graficos de patentes, horarios, meses y excesos exportados como jpg

## [0.4.0] - 2026-04-26

### Added
- Ejercicio 06: Visualizacion del dataframe limpio, y calculo de los porcentajes 
correspondientes a las infracciones en la fecha 1932-01-01 y el porcentaje
de infracciones correspondientes a la hora 00:00.

## [0.5.0] - 2026-04-26

### Added
Redacción de la conclusión del trabajo práctico grupal.

## [0.4.0] - 2026-04-26

### Added
- Ejercicio 06: Visualizacion del dataframe limpio, y calculo de los porcentajes 
correspondientes a las infracciones en la fecha 1932-01-01 y el porcentaje
de infracciones correspondientes a la hora 00:00.

## [0.5.0] - 2026-04-26

### Added
Redacción de la conclusión del trabajo práctico grupal.

## [1.0.0] - 2026-05-19

### Added
- Clone del repositorio Sprint_1
- Creación de rama Sprint_2 partiendo de Sprint_1
- Descarga y extracción del dataset de imágenes en raw/imgs
- Actualización de README al Sprint 2

## [1.1.0] - 2026-05-21

### Added
- Listado de imágenes con nombre y tamaño en KB
- Separación en grupos plates y completes
- Generación del diccionario group_images
- Guardado de group_images en urban_flow/data/interim/group_images.json
- Función reutilizable mostrar_imagenes_grilla

## [1.2.0] - 2026-05-21

### Added
- Conversión a escala de grises de imágenes originales
- Suavizado con GaussianBlur sobre imágenes en escala de grises
- Detección de bordes con Canny sobre imágenes suavizadas
- Visualización de imágenes procesadas en cada etapa

## [1.0.0] - 2026-05-19

### Added
- Clone del repositorio Sprint_1
- Creación de rama Sprint_2 partiendo de Sprint_1
- Descarga y extracción del dataset de imágenes en raw/imgs
- Actualización de README al Sprint 2

## [1.1.0] - 2026-05-21

### Added
- Listado de imágenes con nombre y tamaño en KB
- Separación en grupos plates y completes
- Generación del diccionario group_images
- Guardado de group_images en urban_flow/data/interim/group_images.json
- Función reutilizable mostrar_imagenes_grilla

## [1.2.0] - 2026-05-21

### Added
- Conversión a escala de grises de imágenes originales
- Suavizado con GaussianBlur sobre imágenes en escala de grises
- Detección de bordes con Canny sobre imágenes suavizadas
- Visualización de imágenes procesadas en cada etapa

## [1.3.0] - 2026-05-22

### Added
- Extracción de patentes con EasyOCR sobre grupo plates
- Actualización de group_images.json con campo patent
- Matching de patentes OCR vs speeding_fines.csv (umbral 80%)
- Generación de speeding_fines_image.csv con columnas
  imagen, patente_imagen, ratio

## [1.0.0] - 2026-05-19

### Added
- Clone del repositorio Sprint_1
- Creación de rama Sprint_2 partiendo de Sprint_1
- Descarga y extracción del dataset de imágenes en raw/imgs
- Actualización de README al Sprint 2

## [1.1.0] - 2026-05-21

### Added
- Listado de imágenes con nombre y tamaño en KB
- Separación en grupos plates y completes
- Generación del diccionario group_images
- Guardado de group_images en urban_flow/data/interim/group_images.json
- Función reutilizable mostrar_imagenes_grilla

## [1.2.0] - 2026-05-21

### Added
- Conversión a escala de grises de imágenes originales
- Suavizado con GaussianBlur sobre imágenes en escala de grises
- Detección de bordes con Canny sobre imágenes suavizadas
- Visualización de imágenes procesadas en cada etapa

## [1.3.0] - 2026-05-22

### Added
- Extracción de patentes con EasyOCR sobre grupo plates
- Actualización de group_images.json con campo patent
- Matching de patentes OCR vs speeding_fines.csv (umbral 80%)
- Generación de speeding_fines_image.csv con columnas
  imagen, patente_imagen, ratio

## [1.4.0] - 2026-05-22

### Added
- Cálculo de multas sin imágenes
- Cálculo de multas con imágenes
- Cálculo de imágenes sin match con el dataset
- Cálculo de multas pendientes de pago (IMPAGA)
- Cálculo de multas pendientes de pago con imágenes relacionadas

## [1.4.0] - 2026-05-22

### Added
- Cálculo de multas sin imágenes
- Cálculo de multas con imágenes
- Cálculo de imágenes sin match con el dataset
- Cálculo de multas pendientes de pago (IMPAGA)
- Cálculo de multas pendientes de pago con imágenes relacionadas

## [1.0.0] - 2026-05-19

### Added
- Clone del repositorio Sprint_1
- Creación de rama Sprint_2 partiendo de Sprint_1
- Descarga y extracción del dataset de imágenes en raw/imgs
- Actualización de README al Sprint 2

## [1.1.0] - 2026-05-21

### Added
- Listado de imágenes con nombre y tamaño en KB
- Separación en grupos plates y completes
- Generación del diccionario group_images
- Guardado de group_images en urban_flow/data/interim/group_images.json
- Función reutilizable mostrar_imagenes_grilla

## [1.2.0] - 2026-05-21

### Added
- Conversión a escala de grises de imágenes originales
- Suavizado con GaussianBlur sobre imágenes en escala de grises
- Detección de bordes con Canny sobre imágenes suavizadas
- Visualización de imágenes procesadas en cada etapa

## [1.3.0] - 2026-05-22

### Added
- Extracción de patentes con EasyOCR sobre grupo plates
- Actualización de group_images.json con campo patent
- Matching de patentes OCR vs speeding_fines.csv (umbral 80%)
- Generación de speeding_fines_image.csv con columnas
  imagen, patente_imagen, ratio

## [1.4.0] - 2026-05-22

### Added
- Cálculo de multas sin imágenes
- Cálculo de multas con imágenes
- Cálculo de imágenes sin match con el dataset
- Cálculo de multas pendientes de pago (IMPAGA)
- Cálculo de multas pendientes de pago con imágenes relacionadas

## [1.5.0] - 2026-05-22

### Added
- Análisis reflexivo sobre imágenes y datos en data/Readme.md
