
# 🌍 Proyecto de Clasificación Binaria de Sismos en Tierra del Fuego

Este proyecto tiene como objetivo desarrollar un modelo de aprendizaje automático que permita clasificar eventos sísmicos registrados en la región de Tierra del Fuego, Argentina, en dos categorías: **significativos** (ML ≥ 4.5) y **no significativos**, a partir de características geográficas y técnicas.

## 📌 Objetivo General

Construir un modelo de clasificación binaria que, a partir de datos sísmicos reales, determine si un sismo debe considerarse significativo según su magnitud local (ML) y otros parámetros.

## ⚙️ Herramientas y tecnologías utilizadas

- Python 3.x
- Google Colab
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn (para el modelado)
- Tabula-py (para extracción de datos desde PDF)
- Git y GitHub (para control de versiones)

## 📁 Estructura del proyecto

```
📦sismo-clasificador
 ┣ 📂data
 ┃ ┣ 📄sismos_original.pdf
 ┃ ┣ 📄sismos_completo.xlsx
 ┃ ┗ 📄sismos_preprocesado.csv
 ┣ 📂notebooks
 ┃ ┗ 📄01_extraccion_y_preparacion.ipynb
 ┣ 📂models
 ┃ ┗ 📄modelo_final.pkl
 ┣ 📂reports
 ┃ ┗ 📄informe_final.pdf
 ┣ 📄README.md
 ┗ 📄requirements.txt
```

## 📊 Dataset

Los datos fueron extraídos del sitio oficial del Instituto Nacional de Prevención Sísmica (INPRES). La extracción se realizó desde un archivo PDF con registros detallados de eventos sísmicos en la región.

Características del dataset:
- Fecha y hora del evento
- Coordenadas geográficas (latitud y longitud)
- Profundidad
- Magnitud local (ML)
- Otros datos técnicos complementarios

## 🧠 Enfoque del proyecto

1. **Extracción y limpieza de datos** desde PDF (usando `tabula-py`)
2. **Preprocesamiento**: conversión de tipos, limpieza, creación de variable objetivo (0 = No significativo, 1 = Significativo)
3. **Exploración y visualización** de datos
4. **Entrenamiento de modelos**: SVM, Regresión Logística, Random Forest
5. **Evaluación**: matriz de confusión, accuracy, precision, recall
6. **Conclusiones y recomendaciones**

## 🔄 Estado del proyecto

- [x] Extracción del dataset desde PDF
- [x] Conversión y guardado como Excel
- [ ] Limpieza y preprocesamiento
- [ ] Visualización de datos
- [ ] Modelado y evaluación
- [ ] Redacción del informe final

## 📌 Próximos pasos

- Eliminar valores faltantes y corregir tipos de datos
- Crear la variable objetivo binaria basada en ML
- Aplicar técnicas de visualización geográfica
- Comparar al menos dos algoritmos de clasificación
- Documentar los resultados y subir los modelos

## 📜 Licencia

Proyecto educativo desarrollado como parte de la cursada de **Aprendizaje Automático** en la Tecnicatura Superior en Ciencia de Datos e Inteligencia Artificial – Politécnico Malvinas Argentinas, Tierra del Fuego.
