# Urban Flow

## Sprint actual: Sprint 2

## Objetivo
Determinar qué multas tienen evidencia visual válida, cruzando
el dataset de infracciones procesado en el Sprint 1 con un
dataset de imágenes capturadas por los radares urbanos.

## Introducción y contexto
La localidad de Vaalserberg (Bélgica), ubicada en zona
fronteriza con Países Bajos y Alemania, cuenta con radares
urbanos para detectar infracciones de velocidad.

Los radares generan registros administrativos de multas de forma
automática y las cámaras asociadas registran la evidencia visual
que acompaña y valida la infracción. Sin embargo:

- No todas las multas tienen una imagen asociada.
- No todas las imágenes corresponden a una infracción.
- Puede haber errores de detección.

## Sprints
- Sprint 1: limpieza y análisis del dataset de infracciones.
- Sprint 2: validación de evidencia visual con OpenCV y EasyOCR.
