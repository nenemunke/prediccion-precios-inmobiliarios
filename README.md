# Predicción de Precios Inmobiliarios con Machine Learning

## Descripción
Proyecto de Data Science enfocado en la predicción de precios de viviendas utilizando modelos de **Regresión Lineal Múltiple**. Se trabajó con un dataset inmobiliario para identificar qué características (features) influyen más en el valor final de una propiedad.

## Objetivo
Entrenar un modelo de Machine Learning capaz de predecir el precio de una casa basándose en variables como el área, cantidad de baños y habitaciones, optimizando la precisión del modelo mediante la selección de características.

## Tecnologías
* **Python** (Pandas, Numpy)
* **Scikit-Learn** (Modelado, métricas de evaluación)
* **Matplotlib / Seaborn** (Visualización de datos y correlaciones)

## Resultados
El proyecto se desarrolló en dos iteraciones para medir el impacto de la selección de variables:

1.  **Iteración 1 (Modelo Base):** Se utilizó solo la variable `area`.
    * *R² Score:* 0.19 (El modelo explicaba solo el 19% de la varianza).
2.  **Iteración 2 (Modelo Multivariable):** Se incorporaron variables con alta correlación como `bathrooms` y `bedrooms`.
    * *R² Score:* **0.49** 🚀
    * **Conclusión:** Al enriquecer el modelo con variables arquitectónicas clave, se logró **más que duplicar la precisión predictiva**, demostrando la importancia de la calidad de los datos sobre la complejidad del algoritmo.

## Estructura del Proyecto
* `analisis_exploratorio`: Limpieza de datos y matriz de correlación.
* `entrenamiento`: División del dataset en Training/Test set.
* `evaluacion`: Medición del error cuadrático medio (MSE) y coeficiente de determinación (R²).
