
# Proyecto: Modelado y Evaluación de Clasificación - Churn

## Descripción del proyecto

El objetivo de este proyecto es desarrollar un modelo de Machine Learning de clasificación binaria para predecir si un cliente abandonará un servicio (Churn).

Se utiliza el dataset Telco Customer Churn, que contiene información sobre los clientes, sus servicios contratados y su comportamiento.

## Tecnologías utilizadas

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Dataset

Archivo utilizado: WA_Fn-UseC_-Telco-Customer-Churn.csv   (https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

El conjunto de datos contiene información de clientes de una empresa de telecomunicaciones.

La variable objetivo es Churn:
- No: el cliente permanece en el servicio.
- Yes: el cliente abandona el servicio.

## Desarrollo del proyecto

Se realizaron las siguientes etapas:

1. Carga y exploración de los datos.
2. Limpieza y preparación del dataset.
3. Conversión de variables categóricas a numéricas.
4. División de datos en entrenamiento (80%) y prueba (20%).
5. Entrenamiento del modelo Random Forest.
6. Evaluación mediante métricas de clasificación.
7. Visualización de la matriz de confusión.
8. Interpretación de los resultados.

## Modelo utilizado

Random Forest Classifier, utilizando 100 árboles de decisión.

## Resultados obtenidos

| Métrica | Resultado |
|---|---:|
| Accuracy | 78,96% |
| Precision | 62,58% |
| Recall | 51,87% |
| F1-Score | 56,73% |

## Matriz de confusión

| Valores reales | Predicción No | Predicción Yes |
|---|---:|---:|
| No Churn | 917 | 116 |
| Churn | 180 | 194 |

## Conclusión

El modelo obtuvo un Accuracy aproximado del 78,96%.
Recall es la metrica mas importante, porque permite identificar a los clientes que realmente abandonan el servicio.

Se detectaron 194 clientes que abandonaron el servicio efectivamente, mientras que 180 clientes fueron clasificados demanera erronea como clientes que permanecerían.

Los falsos negativos significan una importante perdida para la empresa, esto se debe porque no se puede analizar bien como aplicar estrategias para mantenerlos en el tiempo.

Por lo que se recomienda es mejorar el Recall para poder detectar de manera efectiva aquellos clientes que quiere abandonar y aplicar las estrategias convenientes.

## Instrucciones de ejecución

1. Abrir Google Colab.
2. Cargar el notebook modelado_metricas.ipynb.
3. Subir el archivo CSV del dataset cuando el notebook lo solicite.
4. Ejecutar las celdas en orden.
5. Consultar las métricas y la matriz de confusión generadas.


