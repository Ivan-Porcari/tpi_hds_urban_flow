 
## Análisis: relación entre imágenes y datos

A partir del cruce entre el dataset de multas y las imágenes
capturadas por los radares urbanos se pueden destacar las
siguientes observaciones:

- **Baja cobertura visual**: de un total de 1713 multas
  registradas, solo 544 cuentan con imagen asociada (32%).
  Esto significa que el 68% de las infracciones (1169 multas)
  no tiene evidencia visual, lo que limita fuertemente la
  capacidad de validación del sistema.

- **Errores de OCR**: de todas las imágenes del grupo plates,
  54 no pudieron vincularse a ninguna multa del dataset. Esto
  refleja las limitaciones del reconocimiento óptico, donde
  caracteres similares (O/0, I/1, B/8) generan falsos negativos
  aun cuando la imagen corresponde a una infracción real.

- **Multas impagas sin respaldo visual**: hay 430 multas con
  estado IMPAGA, pero solo 22 de ellas tienen una imagen
  relacionada. Esto significa que el 95% de las multas
  pendientes de cobro no cuenta con evidencia visual, lo que
  debilita considerablemente su sustento probatorio en caso
  de disputa administrativa o judicial.

- **Conclusión general**: el sistema de radares presenta una
  cobertura fotográfica insuficiente y errores de detección
  que reducen la confiabilidad del dataset. Para mejorar la
  tasa de match sería necesario un modelo de OCR más robusto
  y una mayor consistencia en la captura de imágenes por
  parte de los radares.

## Análisis: relación entre imágenes y datos

A partir del cruce entre el dataset de multas y las imágenes
capturadas por los radares urbanos se pueden destacar las
siguientes observaciones:

- **Baja cobertura visual**: de un total de 1713 multas
  registradas, solo 544 cuentan con imagen asociada (32%).
  Esto significa que el 68% de las infracciones (1169 multas)
  no tiene evidencia visual, lo que limita fuertemente la
  capacidad de validación del sistema.

- **Errores de OCR**: de todas las imágenes del grupo plates,
  54 no pudieron vincularse a ninguna multa del dataset. Esto
  refleja las limitaciones del reconocimiento óptico, donde
  caracteres similares (O/0, I/1, B/8) generan falsos negativos
  aun cuando la imagen corresponde a una infracción real.

- **Multas impagas sin respaldo visual**: hay 430 multas con
  estado IMPAGA, pero solo 22 de ellas tienen una imagen
  relacionada. Esto significa que el 95% de las multas
  pendientes de cobro no cuenta con evidencia visual, lo que
  debilita considerablemente su sustento probatorio en caso
  de disputa administrativa o judicial.

- **Conclusión general**: el sistema de radares presenta una
  cobertura fotográfica insuficiente y errores de detección
  que reducen la confiabilidad del dataset. Para mejorar la
  tasa de match sería necesario un modelo de OCR más robusto
  y una mayor consistencia en la captura de imágenes por
  parte de los radares.
