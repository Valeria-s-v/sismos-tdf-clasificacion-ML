![Clasificación de Sismos](docs/Clasificación%20de%20sismos%20-%20tdf.png)


# 🌍 Proyecto de Clasificación Binaria de Sismos en Tierra del Fuego

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)  
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)](https://scikit-learn.org/)  
[![Estado](https://img.shields.io/badge/estado-final-success)]()  
[![Licencia](https://img.shields.io/badge/licencia-MIT-blue)](LICENSE)

---

Este proyecto de **Machine Learning** tiene como objetivo desarrollar un modelo de aprendizaje automático que permita clasificar eventos sísmicos registrados en la región de Tierra del Fuego, Argentina, en dos categorías: **significativos** (percibidos o con impacto) y **no significativos**, a partir de características geográficas y técnicas.

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
- Pandas, NumPy, Matplotlib
- Scikit-learn
- Tabula-py (extracción de PDF)
- Git y GitHub
- Cooiecutter

Este repositorio incluye:
- 🧹 Limpieza y transformación de datos crudos.
- 📊 Exploración y visualización.
- 🤖 Entrenamiento de modelos: SVM, Regresión Logística y Random Forest.
- 📈 Evaluación con métricas completas y curvas ROC.
- 📋 Interpretación: importancia de variables, matriz de confusión.
- 📂 Organización modular (notebooks, src, modelos, reportes).

---

## 📁 Estructura del proyecto

- `data/` 📊: Dataset original y archivos derivados.
- `docs/` 🖼️: Imagen representativa del proyecto.
- `models/` 
- `notebooks/` 📒: Notebook principal del proyecto.
- `references/` 
- `reports/` 📝: Entregables (PowerPoint, informe).
- `src/` 
- `requirements.txt` 📦: Dependencias de Python.
- `README.md` ✨: Documentación inicial del proyecto.
- `LICENSE` 📄: Licencia MIT del proyecto.

---

## 📊 Dataset

Los datos provienen del documento oficial del Instituto Nacional de Prevención Sísmica (INPRES), complementado con cálculos geográficos y variables derivadas para enriquecer el análisis.

### Fuente:

📄 [`data/catalogo_sismico_INPRES_2021_2024.pdf`](data/catalogo_sismico_INPRES_2021_2024.pdf)


## 🔄 Estado del proyecto

- [x] Extracción de datos desde PDF
- [x] Limpieza inicial y normalización
- [x] Cálculo de distancias geográficas
- [x] Conversión a CSV y carga en repositorio
- [x] Notebook en desarrollo
- [x] Visualizaciones clave
- [x] Evaluación de modelos
- [x] Informe final completo

## 📝 Documentación

- 📘 [Ver informe en PDF](reports/Entrega1_Clasificacion_Sismos_TDF_ValeriaVillegas.pdf)  
- 🎥 [Ver video de presentación](https://drive.google.com/file/d/18r_e2r-BnRkCraiaXUz3D0UuLe656jUY/view?usp=sharing)
- [📘 Ver reporte final del proyecto (PDF)](reports/Reporte_Clasificación_binaria_Tierra_del_Fuego.pdf)
- [🎞️ Ver presentación en PowerPoint (PDF)](reports/PowerPoint_del_proyecto.pdf)

---

## 🧪 Instalación y ejecución

```bash
git clone https://github.com/Valeria-s-v/sismos-tdf-clasificacion-ML.git
cd sismos-tdf-clasificacion-ML
pip install -r requirements.txt

# Abrí el notebook:
jupyter notebook notebooks/clasificacion_sismos.ipynb
```

---

## 📈 Resultados destacados

- ✅ **Random Forest** es el mejor modelo: alta precisión, recall equilibrado, y ROC AUC > 0.9.
- 🧩 **Importancia de variables**: identificamos los factores más influyentes en la percepción de sismos.
- 📊 **Curvas ROC comparadas**: ofrecen una visual clara de la capacidad discriminativa de cada modelo para diferentes umbrales.
- 📉 **Matriz de confusión**: permite evaluar fallos de clasificación en cada clase.

---

## 🧠 Uso práctico

Este proyecto puede ser integrado en proyectos reales de:
- Sistemas de alerta temprana.
- Monitoreo de impacto sísmico.
- Informes geocientíficos y planificación local.

---

## 🧑‍💻 Autora

> **Valeria Villegas** — Estudiante de Ciencia de Datos e IA  
> Politécnico Malvinas Argentinas, Tierra del Fuego, Argentina 🇦🇷

---

## 📜 Licencia

Este proyecto está licenciado bajo la Licencia MIT. Ver el archivo [`LICENSE`](LICENSE).
Proyecto educativo desarrollado en el marco de la materia **Aprendizaje Automático** de la Tecnicatura Superior en Ciencia de Datos e Inteligencia Artificial – Politécnico Malvinas Argentinas, Tierra del Fuego.
