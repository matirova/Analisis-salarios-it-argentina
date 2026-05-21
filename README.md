# Análisis Exploratorio y Modelo Predictivo: Salarios IT Argentina

Este proyecto realiza un análisis integral de punta a punta sobre los datos de la encuesta de salarios del sector tecnológico en Argentina (Sysarmy). El objetivo principal es entender las variables que determinan las brechas salariales y construir un modelo predictivo capaz de estimar el salario neto de un profesional.

## Estructura del Proyecto

El cuaderno de Google Colab se encuentra organizado en las siguientes fases profesionales colapsables:

1. **Limpieza de Datos:** Tratamiento de valores nulos, normalización de strings y filtrado de outliers en salarios.
2. **Análisis Exploratorio de Datos (EDA):** Planteo de hipótesis iniciales y cruce de variables macro (moneda de cobro, impacto del dólar).
3. **Visualización de Datos:** Implementación de histogramas con curvas de densidad (KDE) y gráficos de caja (Boxplots) ordenados para analizar el Seniority y mitigar el texto libre en la variable de Género.
4. **Data Engineering / Feature Engineering:** Exportación de un checkpoint en `.csv` y transformación del dataset a una **estructura ancha** mediante codificación binaria (*One-Hot Encoding*) para capturar las tecnologías e idiomas estrella del mercado de forma limpia.
5. **Machine Learning:** Entrenamiento iterativo de un algoritmo de **Árbol de Decisión (Decision Tree Regressor)**, logrando optimizar el porcentaje de acierto ($R^2$) y analizando el peso de las variables (*Feature Importance*).

## Principales Insights Obtenidos
* Los **Años de Experiencia** representan el factor crítico más pesado para el algoritmo (cerca del 60% de la toma de decisiones).
* La **Modalidad 100% Remota** escaló como la segunda variable más importante, validando la hipótesis de la indexación a presupuestos internacionales o del exterior.
* Se evidenció y mapeó visualmente una brecha salarial real en las medianas al cruzar las variables de género normalizadas.

## Tecnologías Utilizadas
* Python
* Pandas & NumPy
* Seaborn & Matplotlib
* Scikit-Learn (Machine Learning)
