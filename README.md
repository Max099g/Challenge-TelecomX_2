 TelecomX - Parte 2: Predicción de Cancelación (Churn)
Este proyecto es la segunda parte del Challenge de Alura Latam / Oracle Next Education (ONE) sobre análisis de evasión de clientes en la empresa TelecomX.
El objetivo es construir modelos de machine learning que permitan predecir qué clientes tienen mayor probabilidad de cancelar el servicio, usando los datos ya limpios y tratados de la parte 1.

##Contenido
El notebook está dividido en 4 etapas:

**Etapa 1 - Preparación de los datos**
Carga del dataset, eliminación de columnas irrelevantes como el ID del cliente, codificación de variables categóricas con one-hot encoding, verificación del balance de clases y normalización de variables numéricas.

**Etapa 2 - Correlación y selección de variables**
Análisis de la matriz de correlación para identificar qué variables tienen más relación con el churn. Se incluyen boxplots y scatter plots de las variables más relevantes como el tiempo de contrato y el cargo mensual.

**Etapa 3 - Modelado predictivo**
Entrenamiento de 3 modelos de clasificación: Regresión Logística, KNN y Random Forest. Se evalúan con métricas de exactitud, precisión, recall y F1-score, además de matrices de confusión y una revisión de overfitting comparando resultados en train vs test.

**Etapa 4 - Interpretación y conclusiones**
Análisis de importancia de variables por modelo y conclusiones con estrategias de retención basadas en los resultados.

tecnologias que use 
- Python 3
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- Google Colab

## Principales hallazgos

Los factores que más influyen en la cancelación son el tiempo de contrato (clientes nuevos cancelan más), el tipo de contrato (mes a mes tiene mucho más churn), el cargo mensual elevado y el uso de fibra óptica. La Regresión Logística fue el modelo más equilibrado para detectar cancelaciones sin generar demasiadas falsas alarmas.

## Cómo ejecutar

El notebook está pensado para correr en Google Colab. Los datos se cargan automáticamente desde este repositorio, no es necesario subir ningún archivo manualmente.
