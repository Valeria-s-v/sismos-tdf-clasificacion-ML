
# 🌍 Proyecto de Clasificación Binaria de Sismos en Tierra del Fuego

Este proyecto tiene como objetivo desarrollar un modelo de aprendizaje automático que permita clasificar eventos sísmicos registrados en la región de Tierra del Fuego, Argentina, en dos categorías: **significativos** (percibidos o con impacto) y **no significativos**, a partir de características geográficas y técnicas.

## 📌 Objetivo General

Desarrollar un modelo de clasificación binaria capaz de identificar si un evento sísmico puede ser percibido por la población o tener impacto, utilizando variables como magnitud, profundidad, distancia a centros urbanos y características temporales.

## 🎯 Objetivos Específicos

- Recolectar y limpiar datos sísmicos históricos de Tierra del Fuego.
- Calcular la distancia epicentral a las ciudades principales (Ushuaia, Río Grande, Tolhuin).
- Generar la variable binaria "percibido" en función de magnitud y distancia.
- Incorporar variables temporales como día, mes y hora.
- Evaluar distintos algoritmos de clasificación y comparar su rendimiento.
- Comunicar los resultados con visualizaciones e indicadores clave.

## ⚙️ Herramientas y tecnologías utilizadas

- Python 3.x
- Google Colab / Jupyter Notebook
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Tabula-py (extracción de PDF)
- Git y GitHub

## 📁 Estructura del proyecto

```
📦sismos-tdf-clasificacion-ML
 ┣ 📂data
 ┃ ┣ 📄sismos_original.pdf
 ┃ ┣ 📄sismos_completo.xlsx
 ┃ ┗ 📄sismos_completo.csv
 ┣ 📂notebooks
 ┃ ┗ 📄sismos-tdf-clasificacion-ML.ipynb
 ┣ 📂models
 ┃ ┗ 📄modelo_final.pkl
 ┣ 📂reports
 ┃ ┗ 📄Entrega1_Clasificacion_Sismos_TDF_ValeriaVillegas.pdf
 ┣ 📂docs
 ┣ 📂references
 ┣ 📂src
 ┣ 📄README.md
 ┗ 📄requirements.txt
```

## 📊 Dataset

Los datos provienen del documento oficial del Instituto Nacional de Prevención Sísmica (INPRES), complementado con cálculos geográficos y variables derivadas para enriquecer el análisis.

### Fuente:

📄 [`data/catalogo_sismico_INPRES_2021_2024.pdf`](data/catalogo_sismico_INPRES_2021_2024.pdf)

## 🧠 Enfoque del proyecto

1. **Extracción de datos** desde PDF.
2. **Limpieza y preprocesamiento** de columnas.
3. **Creación de variables derivadas** (ciudad más cercana, distancia mínima, temporalidad).
4. **Análisis exploratorio y visualización**.
5. **Entrenamiento de modelos** (LogReg, Árboles, KNN, SVM, Random Forest, XGBoost).
6. **Evaluación con métricas** como accuracy, precision, recall y matriz de confusión.
7. **Documentación y entrega de resultados**.

## 🔄 Estado del proyecto

- [x] Extracción de datos desde PDF
- [x] Limpieza inicial y normalización
- [x] Cálculo de distancias geográficas
- [x] Conversión a CSV y carga en repositorio
- [x] Notebook en desarrollo
- [ ] Visualizaciones clave
- [ ] Evaluación de modelos
- [ ] Informe final completo

## 📝 Documentación

📄 [`reports/Entrega1_Clasificacion_Sismos_TDF_ValeriaVillegas.pdf`](reports/Entrega1_Clasificacion_Sismos_TDF_ValeriaVillegas.pdf)

## 📌 Próximos pasos

- Completar el análisis exploratorio
- Comparar al menos 2-3 modelos de clasificación
- Exportar el modelo final entrenado
- Desplegar visualizaciones clave (mapas, gráficas)
- Redactar y subir el informe final

## 📜 Licencia

Proyecto educativo desarrollado en el marco de la materia **Aprendizaje Automático** de la Tecnicatura Superior en Ciencia de Datos e Inteligencia Artificial – Politécnico Malvinas Argentinas, Tierra del Fuego.
