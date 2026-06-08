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
