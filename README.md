# Predicción de Tumores con Machine Learning

Este proyecto utiliza algoritmos de machine learning para predecir si un tumor es benigno o maligno utilizando un conjunto de datos biomédicos. Se exploran varios modelos de clasificación y se selecciona el mejor en función de su desempeño.

## Contenido del Proyecto

El proyecto incluye los siguientes pasos:

1. **Carga de Datos**: Descarga de un conjunto de datos de OpenML.
2. **Exploración y Preparación de Datos**:
   - Análisis de las dimensiones del dataset.
   - Asignación de nombres descriptivos a las columnas.
   - Visualización de la distribución de clases objetivo.
3. **Entrenamiento de Modelos**:
   - Entrenamiento y evaluación de varios modelos de clasificación:
     - Random Forest
     - Regresión Logística
     - Support Vector Machine (SVM)
     - Gradient Boosting
   - Validación cruzada para comparar el desempeño de los modelos.
4. **Afinación de Hiperparámetros**:
   - Uso de `GridSearchCV` para optimizar los hiperparámetros del modelo Gradient Boosting, seleccionado como el mejor modelo.

## Requisitos

Para ejecutar el proyecto, necesitas las siguientes dependencias:

- Python 3.7+
- Bibliotecas de Python:
  - `openml`
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `seaborn`
  - `matplotlib`

Puedes instalarlas ejecutando:
```bash
pip install openml pandas numpy scikit-learn seaborn matplotlib
```

## Estructura del Notebook

El proyecto está documentado en un notebook de Jupyter. La estructura principal es:

1. **Introducción**: Breve descripción del problema y objetivos.
2. **Carga y Exploración de Datos**:
   - Carga del dataset desde OpenML.
   - Análisis exploratorio inicial (dimensiones, tipos de datos, distribución de clases).
3. **Entrenamiento y Evaluación de Modelos**:
   - Comparación de diferentes modelos mediante métricas como `precision`, `recall` y `F1-score`.
   - Visualización de resultados con gráficos.
4. **Optimización del Mejor Modelo**:
   - Afinación de hiperparámetros usando GridSearchCV para mejorar la precisión del modelo Gradient Boosting.
5. **Conclusiones**: Resumen de los resultados y próximos pasos.

## Uso

Sigue estos pasos para ejecutar el notebook:

1. Clona el repositorio:
   ```bash
   git clone https://github.com/Unai1117/BreastCancerBenignOrMalig.git
   ```

2. Cambia al directorio del proyecto:
   ```bash
   cd BreastCancerBenignOrMalig
   ```

3. Abre el notebook en Jupyter:
   ```bash
   jupyter notebook tumor_prediction.ipynb
   ```

4. Ejecuta las celdas secuencialmente para reproducir el análisis y resultados.

## Resultados

El modelo optimizado (Gradient Boosting) logró los siguientes resultados:

- **Métricas principales**:
  - Precisión: 98%
  - Recall: 97%
  - F1-Score: 97%

Puedes encontrar más detalles en la sección de afinación de hiperparámetros y en los reportes de clasificación generados por los modelos.

## Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar el proyecto o agregar nuevas funcionalidades, sigue estos pasos:

1. Haz un fork del repositorio.
2. Crea una rama para tu nueva funcionalidad:
   ```bash
   git checkout -b nueva_funcionalidad
   ```
3. Realiza tus cambios y haz un commit:
   ```bash
   git commit -m "Descripción de los cambios"
   ```
4. Envía tus cambios mediante un pull request.

