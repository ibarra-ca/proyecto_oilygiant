# 🛢 Predictions for OilyGiant

El objetivo del proyecto fue ayudar a **OilyGiant**, una compañía de extracción de petróleo, a identificar las regiones más rentables para la apertura de **200 nuevos pozos petrolíferos**, basándose en datos geológicos y de producción histórica.

👉 [**Ver análisis completo**](https://ibarra-ca.github.io/Predictions-for-OilyGiant/)

---

## 🎯 Objetivo del proyecto
Construir un modelo de *machine learning* capaz de **predecir el volumen de reservas de petróleo** en pozos nuevos, estimar la rentabilidad esperada y seleccionar la región con el **mayor margen de beneficio ajustado por riesgo**.  
El análisis incluye la simulación de beneficios esperados mediante **técnicas de bootstrapping** para evaluar la variabilidad e incertidumbre de las ganancias.

---

## 🧪 Metodología y pasos realizados

### 1️⃣ Exploración y comprensión de los datos
- Se analizaron los parámetros de pozos petrolíferos de **tres regiones distintas**, incluyendo:
  - Calidad del crudo (características geológicas).
  - Volumen de reservas.
  - Coordenadas o identificadores de pozos.
- Verificación de consistencia, normalidad y correlaciones entre variables.

### 2️⃣ Limpieza y preprocesamiento
- Estandarización de datos y normalización de variables predictoras.
- Separación de conjuntos de entrenamiento, validación y prueba por región.
- Eliminación de outliers y chequeo de sesgos regionales.

### 3️⃣ Entrenamiento del modelo predictivo
- Entrenamiento de un modelo de **regresión lineal** para predecir el volumen de reservas en pozos nuevos.
- Evaluación de métricas como:
  - **RMSE** (Root Mean Squared Error)
  - **MAE** (Mean Absolute Error)
  - Correlación entre valores reales y predichos
- Validación cruzada para evitar sobreajuste y asegurar generalización entre regiones.

### 4️⃣ Selección de los mejores pozos
- Predicción del volumen de reservas en cada pozo potencial.
- Selección de los **200 pozos con los valores estimados más altos** en cada región.
- Cálculo del beneficio total proyectado considerando costos operativos y precios del barril.

### 5️⃣ Análisis de beneficios y riesgos
- Simulación de la distribución de beneficios mediante **bootstrapping** (1000 repeticiones).
- Cálculo de:
  - **Beneficio promedio esperado**
  - **Intervalo de confianza del 95%**
  - **Riesgo de pérdidas (probabilidad de rentabilidad negativa)**
- Comparación entre regiones para elegir la más estable y rentable.

---

## 📊 Resultados
- El modelo logró **buen desempeño predictivo (bajo RMSE)** en todas las regiones.  
- Se seleccionaron las **200 ubicaciones más prometedoras** por región, evaluando el beneficio total.  
- El análisis de bootstrapping permitió:
  - Cuantificar la incertidumbre del beneficio.
  - Estimar el riesgo de pérdidas.
  - Identificar la región óptima que maximiza el **beneficio medio** y minimiza la **volatilidad**.

📈 **Conclusión:**  
La región seleccionada ofreció el **mayor beneficio esperado con bajo riesgo**, evidenciando el potencial del modelo para apoyar decisiones estratégicas de inversión en exploración petrolera.

---

## ⚙️ Tecnologías utilizadas
| Categoría | Herramientas |
|------------|---------------|
| Lenguaje | Python |
| Librerías para datos | Pandas · NumPy |
| Modelado | Scikit-learn (LinearRegression) |
| Evaluación | RMSE · MAE · Bootstrap Simulation |
| Visualización | Matplotlib · Seaborn |
| Entorno | Jupyter Notebook |

---

## 📈 Visualizaciones incluidas
- Distribuciones de volumen de reservas por región.  
- Correlación entre características geológicas y reservas.  
- Comparación de métricas de error por modelo.  
- Curvas de beneficio esperado y riesgo por región.  
- Histogramas de simulación de beneficios (bootstrapping).  

🔗 **Explora el análisis completo aquí:**  
👉 [https://ibarra-ca.github.io/Predictions-for-OilyGiant/](https://ibarra-ca.github.io/Predictions-for-OilyGiant/)

---

## 🧩 Conclusiones
- El modelo de regresión lineal predice eficazmente el volumen de reservas y facilita la evaluación económica de nuevas perforaciones.  
- La simulación mediante *bootstrapping* permite estimar no solo el beneficio esperado, sino también el riesgo asociado a la decisión.  
- Este enfoque basado en datos proporciona una herramienta objetiva para priorizar regiones en función de su **rentabilidad ajustada al riesgo**.  

---

## 🚀 Aprendizajes clave
- Aplicación de *machine learning* en escenarios de toma de decisiones económicas y geológicas.  
- Valor del análisis de riesgo mediante *bootstrapping* en problemas de incertidumbre.  
- Importancia del equilibrio entre beneficio esperado y riesgo para optimizar decisiones de inversión.

---

📘 **Autor:** Carlos Ibarra  
🔗 [GitHub](https://github.com/ibarra-ca) · [LinkedIn](https://www.linkedin.com/in/carlos-armado-ibarra-del-ángel)
