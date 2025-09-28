# churn_analysis

Análisis de churn de clientes con ML, explorando el impacto del preprocesamiento y la explicabilidad de los resultados.

## Descripción
Este proyecto consiste en un análisis completo del churn (abandono de clientes) utilizando técnicas de Machine Learning. Se centra en:

- **Preprocesamiento de datos:** Evaluación del impacto de distintas técnicas de limpieza, transformación y escalado sobre los modelos.
- **Modelado:** Comparación de diferentes algoritmos de Machine Learning (KNN y árboles de decisión) para predecir la probabilidad de abandono.
- **Exploración y explicabilidad:** Análisis exploratorio de los datos y explicación de los resultados para identificar los factores que más influyen en el churn.

El proyecto fue realizado como parte de la asignatura **Minería de Datos**.

## Contenido del repositorio
- `data/` → Contiene el dataset utilizado.  
- `analisis_datos.ipynb` → Notebook con análisis exploratorio, preprocesamiento y modelos de ML.  
- `memoria.pdf` → Documento con los resultados del análisis y la explicación detallada de los modelos, interpretabilidad y conclusiones del proyecto.  
- `README.md` → Descripción del proyecto.

## Requisitos y librerías

Este proyecto utiliza Python y las siguientes librerías principales:

- **Estándar:** `random`, `warnings`, `math`, `itertools.chain`, `itertools.combinations`  
- **Ciencia de datos y visualización:** `numpy`, `pandas`, `matplotlib.pyplot`, `seaborn`  
- **Preprocesamiento de datos:**  
  - de `sklearn.compose`: `ColumnTransformer`  
  - de `sklearn.preprocessing`: `StandardScaler`, `MinMaxScaler`, `QuantileTransformer`, `PolynomialFeatures`, `PowerTransformer`  
  - de `sklearn.impute`: `SimpleImputer`, `KNNImputer`  
  - de `category_encoders`: codificadores categóricos  
  - de `sklearn.decomposition`: `PCA`  
- **Selección de características (sklearn.feature_selection):** `SelectKBest`, `f_classif`, `SelectPercentile`, `RFE`, `RFECV`, `SequentialFeatureSelector`  
- **Modelos de Machine Learning:** `KNeighborsClassifier`, `DecisionTreeClassifier` (de `sklearn`)  
- **Evaluación y modelado (sklearn.model_selection y base):** `cross_val_score`, `StratifiedKFold`, `RandomizedSearchCV`, `BaseEstimator`, `TransformerMixin`  
- **Remuestreo de datos desbalanceados (imblearn):** `Pipeline`, `SMOTE`, `RandomOverSampler`, `ADASYN`, `EditedNearestNeighbours`, `RepeatedEditedNearestNeighbours`, `AllKNN`, `TomekLinks`, `RandomUnderSampler`, `SMOTEENN`, `SMOTETomek`  
- **Algoritmos evolutivos (DEAP):** `base`, `creator`, `tools`, `algorithms`  
- **Explicabilidad de modelos:** `shap`  

## Clonar el repositorio

```bash
git clone https://github.com/tu_usuario/churn_analysis.git
