# Análisis de Churn con Python

Este repositorio contiene un análisis exhaustivo de la pérdida de clientes en un banco, realizado utilizando Python y varias bibliotecas de ciencia de datos.

## Descripción General del Proyecto

El objetivo de este proyecto fue explorar un conjunto de datos de información de clientes bancarios para identificar los factores clave que influyen en la pérdida de clientes (la decisión de abandonar el banco). El análisis incluye la limpieza de datos, el análisis exploratorio de datos (EDA), la ingeniería de características y el desarrollo y la evaluación de modelos de aprendizaje automático para predecir la pérdida de clientes.

## Hallazgos Clave

El análisis reveló varios factores importantes asociados con la pérdida de clientes:

* **Geografía:** Los clientes en Alemania muestran una tasa de pérdida significativamente mayor en comparación con los de Francia y España.
* **Edad:** Los clientes de mediana edad (aproximadamente entre 40 y 59 años) muestran una mayor propensión a la pérdida de clientes.
* **Actividad del Cliente:** Los miembros inactivos tienen más probabilidades de abandonar que los miembros activos.
* **Número de Productos:** Los clientes con 1 o 3-4 productos bancarios tienden a tener tasas de pérdida más altas.
* **Saldo en Cuenta:** Los clientes con saldo cero también presentan una tasa de pérdida notable.

## Metodología

Los siguientes pasos se llevaron a cabo en el análisis:

1.  **Limpieza y Preprocesamiento de Datos:**
    * Se manejaron los valores faltantes (Ninguno en este conjunto de datos).
    * Se eliminaron las columnas irrelevantes (`RowNumber`, `CustomerId`, `Surname`).
    * Se codificaron las variables categóricas.
    * Se escalaron las variables numéricas.
2.  **Análisis Exploratorio de Datos (EDA):**
    * Se realizó un análisis univariado para comprender la distribución de las variables individuales.
    * Se llevó a cabo un análisis bivariado para explorar las relaciones entre las variables predictoras y la variable objetivo (`Exited`).
    * Se visualizaron los datos utilizando histogramas, diagramas de caja, gráficos de barras y gráficos interactivos.
3.  **Ingeniería de Características:**
    * Se crearon nuevas características para capturar las interacciones entre las variables (por ejemplo, `Age_Geography`, `Products_Activity`).
    * Se crearon variables agrupadas (`Age_Group`, `Balance_Group`).
4.  **Desarrollo y Evaluación del Modelo:**
    * Se comparó el rendimiento de varios modelos de aprendizaje automático (Regresión Logística, Árbol de Decisión, Random Forest, Gradient Boosting).
    * Se ajustaron los hiperparámetros utilizando GridSearchCV.
    * Se evaluó el modelo de mejor rendimiento (Gradient Boosting) utilizando métricas como accuracy, precision, recall, F1-score y AUC ROC.

## Rendimiento del Modelo

El modelo de Gradient Boosting logró el mejor rendimiento, con un AUC ROC de 0.8611. Sin embargo, el modelo mostró algunas dificultades para predecir con precisión la pérdida de clientes para los clientes que realmente abandonaron (menor precisión para la clase de abandono).

## Recomendaciones

Según el análisis, se proponen las siguientes recomendaciones:

* **Estrategias de Retención Dirigidas:** Implementar estrategias de retención específicas para los segmentos de clientes de alto riesgo (por ejemplo, clientes en Alemania, miembros inactivos, clientes de mediana edad).
* **Mejoras en Productos y Servicios:** Investigar y abordar las razones detrás de la alta tasa de abandono entre los clientes con 1 o 3-4 productos.
* **Predicción Proactiva de Abandono:** Utilizar el modelo desarrollado para identificar de forma proactiva a los clientes con riesgo de abandono y ofrecer intervenciones personalizadas.

## Cómo Empezar

1.  Clonar el repositorio: `git clone https://github.com/TuUsuarioDeGitHub/analisis-churn-python.git`
2.  Navegar al repositorio: `cd analisis-churn-python`
3.  (Opcional) Crear un entorno virtual: `python3 -m venv .venv` y activarlo: `source .venv/bin/activate`
4.  Instalar las bibliotecas necesarias: `pip install -r requirements.txt`
5.  Abrir y ejecutar el Jupyter Notebook: `notebooks/analisis_churn.ipynb`

## Bibliotecas Utilizadas

* Pandas
* NumPy
* Matplotlib
* Seaborn
* scikit-learn
* Plotly

## Autor


Yesio11
