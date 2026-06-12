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
- Incorporación del archivo speeding_fines.csv a la carpeta raw
- Carga de dataset speeding_fines.csv mediante pathlib
- Análisis de tipo (dtypes) y valores nulos (isnull().sum())

## [0.3.0] - 2026-04-24

### Added
- Normalización de fechas, horas, ubicaciones y patentes
- Eliminación de filas con inconsistencias
- Búsqueda de outliers en columnas numéricas
- Creación de columnas exceso_velocidad_real y exceso_velocidad
- Generación de dataset limpio en carpeta interim

## [0.4.0] - 2026-04-26

### Added
- Clase FineAnalyzer con 5 métodos de análisis
- Gráficos exportados como jpg
- Visualización del dataframe limpio y cálculo de porcentajes

## [0.5.0] - 2026-04-26

### Added
- Redacción de la conclusión del trabajo práctico grupal

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

## [1.6.0] - 2026-06-08

### Fixed
- Corrección del algoritmo de similitud en calcular_ratio:
  se reemplazó LCS por comparación posicional estricta
  de izquierda a derecha, alineando la lógica con la
  consigna del ejercicio 04

## [1.7.0] - 2026-06-08

### Fixed
- Corrección de matching_patentes: ahora genera el CSV completo
  con todas las multas, agregando imagen, patente_imagen y ratio
  solo cuando existe match >= 80%

## [2.0.0] - 2026-06-08

### Added
- Creación de rama Sprint_3 partiendo de Sprint_2
- Verificación de acceso a todos los datasets previos
- Actualización de README al Sprint 3

## [2.1.0] - 2026-06-09

### Added
- Inicialización de DVC en el repositorio
- Creación de remote DVC local en /content/remote_dvc
- Migración de speeding_fines_image.csv a DVC
- Migración de imágenes (urban_flow/data/raw/imgs) a DVC
- Push de datos al remote DVC

## [2.2.0] - 2026-06-09

### Added
- Exploración del CSV base speeding_fines_image.csv
- Diseño del modelo lógico con entidades Vehiculo,
  Radar, Multa y Evidencia

## [2.3.0] - 2026-06-10

### Added
- Clases del modelo lógico: Vehiculo, Radar,
  Evidencia y Multa
- Función procesar_fila_csv que mapea una fila
  del CSV a instancias del modelo lógico

## [2.4.0] - 2026-06-10

### Added
- Modelos relacionales SQLAlchemy: VehiculoORM,
  RadarORM, EvidenciaORM y MultaORM
- Claves primarias y foráneas definidas
- Relaciones entre tablas con relationship()
- Método __repr__ en cada modelo

## [2.5.0] - 2026-06-10

### Added
- Creación de base de datos SQLite transito.db
- Creación automática de tablas con SQLAlchemy ORM
- Migración de datos desde speeding_fines_image.csv
- Validación de registros: 66 vehículos, 4 radares,
  1713 multas, 29 evidencias
- transito.db migrado a DVC

## [2.6.0] - 2026-06-12

### Added
- Consultas SQL: top patentes con más multas
- Consultas SQL: multas sin evidencia asociada
- Consultas SQL: radares más activos
- Consultas SQL: reincidentes en período dado
- Consultas SQL: porcentaje de multas con evidencia visual

## [2.7.0] - 2026-06-12

### Added
- Base vectorial ChromaDB 'patente_vectorial'
- Embeddings OpenCLIP de imágenes de evidencia
- Vinculación de imágenes con patente del vehículo
