# Objetivo

Desarrollar y comparar modelos predictivos basados en Regresión Lineal Múltiple y Árboles de Decisión para estimar los tiempos de operación de diferentes piezas a partir de sus características técnicas (aquí se evaluan tres familias de productos representadas en cada base de datos ) .

El propósito es identificar cuál de los dos modelos ofrece un mejor desempeño predictivo y puede utilizarse como herramienta de apoyo para la planificación de la producción, la estimación de capacidad y la toma de decisiones operativas.

Las variables analizadas incluyen características como el área de la pieza en decímetros cuadrados, el tipo de material y otros atributos relevantes que influyen en el tiempo requerido para realizar la operación.

## Metodología

1. **Carga de datos**
   - Importación de las bases de datos previamente depuradas y preparadas para el análisis.

2. **Análisis exploratorio de datos (EDA)**
   - Exploración de las variables disponibles.
   - Identificación de patrones, distribuciones y posibles relaciones entre variables.
   - Selección preliminar de las características con potencial influencia sobre el tiempo de operación.

3. **Análisis de correlación**
   - Cálculo de coeficientes de correlación, incluyendo Pearson y coeficiente R.

4. **Desarrollo y entrenamiento de modelos**
   - Construcción de un modelo de Regresión Lineal Múltiple.
   - Construcción de un modelo basado en Árboles de Decisión.

5. **Evaluación y comparación de modelos**
   - Comparación del desempeño de los modelos mediante métricas de ajuste y error.
   - Identificación del modelo con mayor capacidad predictiva para estimar tiempos futuros.

6. **Análisis de sobreajuste (Overfitting)**
   - Comparación del desempeño entre datos de entrenamiento y prueba.
  
## Hallazgos Principales
1. Los decímetros cuadrados son la variable con mayor influencia sobre el tiempo de operación

El análisis exploratorio y los coeficientes de correlación evidenciaron que el área de la pieza, medida en decímetros cuadrados, es la característica que más impacta el tiempo requerido para realizar la operación. Adicionalmente, se observaron altos niveles de correlación dentro de cada familia de productos, lo que sugiere que los procesos cuentan con una adecuada estandarización y consistencia operativa.

2. El modelo de Árboles de Decisión presentó el mejor desempeño predictivo

Tras comparar los modelos de Regresión Lineal Múltiple y Árboles de Decisión, se encontró que el modelo basado en Árboles de Decisión se adapta mejor al comportamiento real de los datos. Su capacidad para capturar relaciones no lineales permitió obtener predicciones más precisas, convirtiéndolo en la alternativa seleccionada para estimar los tiempos de futuros productos.

3. No se evidenció un sobreajuste significativo

El análisis de sobreajuste mostró un comportamiento consistente entre los datos de entrenamiento y prueba. Esto indica que el modelo posee una adecuada capacidad de generalización y que las variables seleccionadas explican de manera efectiva la variabilidad de los tiempos de operación. Asimismo, no se identificaron ramas del árbol sustentadas en cantidades reducidas de datos que pudieran comprometer la confiabilidad de las predicciones.

## Conclusión

El estudio permitió identificar que las características físicas de las piezas, especialmente los decímetros cuadrados, son determinantes en la estimación de los tiempos de operación. Tras comparar diferentes enfoques de modelado, el Árbol de Decisión demostró ser la alternativa con mejor capacidad predictiva y de adaptación a los datos reales del proceso. Además, la ausencia de sobreajuste significativo respalda la confiabilidad del modelo para estimar tiempos de nuevos productos, convirtiéndolo en una herramienta útil para la planificación de la producción, la estandarización de procesos y la toma de decisiones basada en datos.
