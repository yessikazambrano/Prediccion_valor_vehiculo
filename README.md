# 🚗 Predicción del valor de vehículos con LightGBM

Este proyecto desarrolla un modelo de regresión para estimar el valor de mercado de coches usados, como parte de una solución para la app **Rusty Bargain**, empresa dedicada a la venta de vehículos de segunda mano.  

El objetivo principal fue ofrecer a los usuarios una **estimación confiable del precio de su coche**, basada en datos históricos, especificaciones técnicas y versión.

---

## 📐 Metodología
- **Preparación de datos**  
  - Limpieza de registros nulos y outliers.  
  - Codificación de variables categóricas (marca, modelo, versión).  
  - Normalización de variables numéricas como kilometraje y año de fabricación.  

- **División del dataset**  
  - Train/Test split en proporción 80/20.  
  - Validación cruzada para garantizar estabilidad en los resultados.  

- **Modelos evaluados**  
  - **Regresión Lineal**: baseline para medir mejoras.  
  - **Árbol de Decisión**: modelo interpretable pero limitado en generalización.  
  - **Random Forest**: robusto y capaz de manejar alta dimensionalidad.  
  - **LightGBM**: modelo final, optimizado con *GridSearchCV* para hiperparámetros clave (learning rate, max depth, n_estimators).  

---

## 📊 Resultados obtenidos
- **Mejor modelo:** LightGBM  
- **RMSE:** 1738.39 → error promedio bajo en la estimación de precios.  
- **Tiempo de entrenamiento:** muy bajo → eficiente para grandes volúmenes de datos.  
- **Velocidad de predicción:** alta → ideal para aplicaciones en tiempo real.  

---

## ✨ Contribuciones del modelo
- Estimaciones precisas y rápidas del valor de vehículos usados.  
- Comparación de distintos algoritmos para seleccionar la mejor opción.  
- Solución escalable y eficiente para aplicaciones de compraventa de coches.  

---

## 📌 Interpretación técnica
El modelo **LightGBM** superó a los demás algoritmos en precisión y eficiencia, gracias a su capacidad para manejar grandes volúmenes de datos y variables categóricas de forma óptima.  
El bajo RMSE demuestra que las predicciones se acercan significativamente al valor real de mercado, mientras que la velocidad de entrenamiento y predicción lo convierten en una solución viable para plataformas de compraventa que requieren respuestas inmediatas.  

---

⭐ **Conclusión:** Este proyecto demuestra cómo los modelos de Machine Learning pueden transformar la experiencia de los usuarios en plataformas de venta de vehículos, ofreciendo estimaciones confiables y rápidas del valor de mercado.  
