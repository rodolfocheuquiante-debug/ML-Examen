# Título del Proyecto: Predicción de Empleabilidad y Éxito en la Carrera Estudiantil.

### Descripción: 

En este repositorio presento el desarrollo completo de mi examen de Machine Learning aplicado. Para este proyecto, procesé un conjunto de datos de 50.000 registros, realicé un análisis exploratorio exhaustivo, implementé técnicas de reducción de dimensionalidad con PCA, agrupé perfiles mediante K-Means y entrené modelos predictivos supervisados, logrando destacar el rendimiento óptimo del modelo Ridge Regression con un ‭$R^2 = 1.0000$‬‭‬.
### Estructura del Repositorio:
* **notebook_examen.ipynb**: Cuaderno principal de Google Colab donde desarrollé todo el flujo técnico, análisis exploratorio, modelado y las justificaciones teóricas del examen.
* **comparativa_modelos.csv**: Archivo que contiene la tabla consolidada con las métricas de rendimiento y los tiempos de ejecución que obtuve al comparar Ridge con Random Forest.
* **requirements.txt**: Archivo de dependencias con las librerías y versiones exactas que utilicé para asegurar la correcta ejecución del código.


## Descripción del Dataset y Tarea

* Dataset: Student Career Success Prediction Dataset en Kaggle (o el enlace correspondiente a tu fuente de datos), compuesto por 50.000 registros y múltiples variables sociodemográficas, académicas y de desempeño laboral de estudiantes.
* Tipo de Tarea: Aprendizaje Supervisado (Regresión) y Aprendizaje No Supervisado (Clustering y Reducción de Dimensionalidad). El objetivo principal es predecir el puntaje de empleabilidad (Employability_Score) de los alumnos y segmentar perfiles de éxito laboral.
### Metodología Resumida

  1. Análisis Exploratorio (EDA): Verificación de nulos, tratamiento de valores atípicos mediante el método IQR en la variable objetivo y estudio de distribuciones.
  3. Preprocesamiento: Escalado de variables numéricas (StandardScaler) y codificación de variables categóricas (OneHotEncoder, OrdinalEncoder), estructurando un espacio de 63 características sin fuga de datos.
  4. Reducción de Dimensionalidad: Aplicación de Análisis de Componentes Principales (PCA) para optimizar la representación espacial de los datos.
  5. Clustering: Búsqueda del ‭$K$‬ óptimo apoyada en el Silhouette Score (‭$K=2$‬‭‬), logrando separar de forma natural a los estudiantes de alto vs. bajo rendimiento.
  6. Modelado Predictivo: Optimización de hiperparámetros mediante GridSearchCV (validación cruzada con cv=5) comparando Ridge Regression frente a Random Forest.
  
## Resultados del Mejor Modelo (Ridge)

| Modelo | RMSE | MAE | R² | MAPE | Tiempo de Ejecución |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Ridge Regression** | **0.0000** | **0.0000** | **1.0000** | **0.0000** | **1.37 s** |
| **Random Forest** | 2.8350 | 2.1185 | 0.9876 | 0.0103 | 1129.21 s |

  * Hallazgo clave: El modelo Ridge demostró precisión matemática absoluta y una eficiencia computacional abismal frente a las 18 horas/minutos de los métodos basados en árboles, consolidándose como la solución definitiva.
###Video Explicativo
Puedes revisar la presentación y defensa completa del proyecto en el siguiente enlace:

