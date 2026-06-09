# Objetivo

Analizar el comportamiento histórico de los precios internacionales del petróleo durante el período 2010-2026 mediante técnicas de análisis exploratorio de datos y series temporales. El proyecto busca identificar tendencias, periodos de alta volatilidad y los años con mayores incrementos o disminuciones en el precio.

Adicionalmente, se evalúa el impacto de acontecimientos económicos, geopolíticos y sociales —como conflictos internacionales, decisiones de producción y la pandemia de COVID-19— sobre la evolución del mercado petrolero. Finalmente, se desarrollan modelos de pronóstico basados en procesos autorregresivos (AR) y ARIMA para estimar el comportamiento futuro de los precios y comparar su capacidad predictiva.


## Información 
- brent_price = valor de referencia internacional para el petróleo extraído del Mar del Norte.
- wti_price = Referente de precios para el mercado estadounidense y uno de los más importantes a nivel mundial.
-	dxy_index = Indicador financiero que mide el valor del dólar estadounidense frente a una cesta de seis monedas extranjeras frente de precios para el mercado estadounidense y uno de los más importantes a nivel mundial.
-	Vix = Conocido popularmente como el "índice del miedo". Mide la volatilidad esperada del mercado de acciones estadounidense
-	brent_return: Rendimiento o variación porcentual del precio del Brent en un periodo determinado.
-	wti_return: Rendimiento o variación porcentual del precio del WTI.
-	brent_lag_1 / brent_lag_3 / brent_lag_7: Precio del Brent con rezago de 1, 3 y 7 días
-	wti_lag_7: Precio del WTI con rezago de 7 días.
-	brent_volatility_7d / brent_volatility_30d: Volatilidad del Brent calculada en ventanas de 7 y 30 días, mide la variación y riesgo del precio.
-	wti_volatility_7d / wti_volatility_30d: Volatilidad del WTI en ventanas de 7 y 30 días.
-	brent_wti_spread: Diferencia de precios entre Brent y WTI, indicador de tensiones regionales y costos de transporte.
-	event_type: Tipo de evento geopolítico o económico registrado (ejemplo: sanción, conflicto, acuerdo).
-	event_description: Descripción detallada del evento que afecta al mercado.
-	event_severity: Grado de impacto del evento (leve, moderado, severo).
-	event_flag: Indicador binario que señala si un evento relevante ocurrió en esa fecha

## Metodología

1. **Carga y preparación de datos**

   * Revisión de la estructura de los datos y validación de la información disponible.

2. **Limpieza de datos**

   * Identificación y tratamiento de valores faltantes o registros inconsistentes.

3. **Análisis exploratorio de datos**

   * Obtención de estadísticas descriptivas de la serie.
   * Identificación de los años con mayores incrementos y disminuciones en el precio del petróleo.
   * Análisis de la evolución histórica de los precios.

4. **Visualización de datos**

   * Construcción de gráficos de precios a lo largo del tiempo.
   * Identificación visual de tendencias, cambios bruscos y periodos de alta volatilidad.
   * Marcación de acontecimientos relevantes, como la pandemia de COVID-19 y otros eventos geopolíticos con impacto en el mercado energético.

5. **Modelado con procesos autorregresivos (AR)**

   * Construcción y entrenamiento de un modelo Autorregresivo (AR).

6. **Modelado ARIMA**
 
   * Construcción y entrenamiento de un modelo ARIMA para realizar pronósticos futuros.
  
  ## Hallazgos Principales

### 1. Tendencia histórica del precio del petróleo

El análisis histórico permitió identificar que el año 2012 presentó uno de los mayores incrementos en el precio del petróleo dentro del periodo estudiado. Asimismo, al evaluar la evolución de largo plazo, se observan periodos de disminución significativa y una alta volatilidad asociada a cambios en las condiciones del mercado global.

### 2. Impacto de eventos geopolíticos y económicos

Los resultados evidencian que acontecimientos geopolíticos, económicos y sociales tienen una influencia directa sobre el comportamiento del mercado petrolero. Eventos como conflictos internacionales, cambios en la producción mundial y la pandemia de COVID-19 generaron variaciones abruptas en los precios, creando puntos de quiebre que modificaron temporalmente la tendencia de la serie.

### 3. Presencia de patrones temporales en los datos

El análisis de la serie temporal permitió identificar la existencia de componentes de tendencia y estacionalidad que afectan el comportamiento de los precios. Estos patrones sugieren que la dinámica del mercado no puede explicarse únicamente mediante observaciones recientes, sino que depende de factores históricos acumulados.

### 4. ARIMA como modelo de pronóstico más adecuado

La comparación entre los modelos de pronóstico mostró que un enfoque exclusivamente Autorregresivo (AR) tiende a presentar mayores errores de estimación debido a la naturaleza de la serie. En contraste, el modelo ARIMA logró capturar de mejor manera la estructura temporal de los datos, proporcionando pronósticos más consistentes y precisos para la estimación futura del precio del petróleo.

## Conclusión

El análisis de la evolución del precio del petróleo entre 2010 y 2026 evidenció que este mercado está altamente influenciado por factores económicos, sociales y geopolíticos, los cuales pueden generar cambios abruptos en su comportamiento y alterar tendencias previamente establecidas. La identificación de periodos de crecimiento, disminución y alta volatilidad permitió comprender mejor la dinámica histórica de la serie y el impacto de acontecimientos globales sobre los precios.

Asimismo, el estudio confirmó la presencia de patrones temporales que deben ser considerados en cualquier ejercicio de pronóstico. La comparación de modelos demostró que ARIMA ofrece un mejor desempeño que un modelo puramente autorregresivo, al capturar de manera más efectiva la estructura de la serie y reducir errores de estimación. En consecuencia, ARIMA se presenta como una herramienta más confiable para apoyar la proyección de precios futuros y el análisis de escenarios en mercados altamente sensibles a factores externos.





