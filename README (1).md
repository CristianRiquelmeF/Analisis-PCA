
> Descubriendo estructuras ocultas: Reducción de dimensionalidad con PCA

**Objetivo:** Aplicar PCA en un conjunto de datos multivariado, interpretar los resultados, visualizar la proyección en 2D, y reflexionar sobre el impacto de la reducción de dimensionalidad en el análisis exploratorio de datos y la preparación de modelos predictivos.



**1.Carga y preprocesamiento de Dataset**

**2.PCA con Scikit-learn**

**3.Visualización de datos en 2D**

- PCA ha logrado transformar un espacio de 8 dimensiones a 2 con pérdida mínima de información relevante para la variabilidad.

- Esta representación puede ser útil para visualizar tendencias, detectar valores atípicos o preparar modelos que usen solo las primeras PCs para simplificar.

- Los agrupamientos no son categóricos sino graduales, lo que es coherente con que el target es continuo.

- Los loadings (cargas) indican cómo contribuye cada variable original a cada Componente Principal (PC). Valores cercanos a ±1 indican una influencia fuerte, mientras que valores cercanos a 0 indican poca relevancia.
- Si PC1 y PC2 ya explican ~50% de la varianza, podrían usarse para:
Visualizar tendencias geográficas (ej: precios altos en zonas costeras).
Clasificar tipos de vivienda (ej: grandes vs. antiguas).


**4.Interpretación de resultados**
- ¿Cuánta información conserva el nuevo espacio?
   
     -Con 2 componentes (PC1 + PC2): Se conserva ~48.9% de la varianza original.
Esto significa que se pierde más del 50% de la información al reducir a 2D.
Puede ser suficiente para visualización, pero insuficiente para modelado predictivo preciso.

- ¿Se observan agrupamientos o patrones más claros?

   -Se observa que los puntos no están mezclados aleatoriamente. Hay una gradación del color (y por tanto del valor del target) que podría indicar que los valores más bajos y más altos tienden a agruparse en regiones diferentes del espacio PCA. Esto sugiere que las componentes principales capturan patrones relacionados con el valor de la vivienda.
Sin embargo, no se forman grupos muy separados o clusters definidos, sino un gradiente.


