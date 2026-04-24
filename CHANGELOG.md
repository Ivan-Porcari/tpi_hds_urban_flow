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
