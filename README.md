![Clasificación de Sismos](docs/Clasificación%20de%20sismos%20-%20tdf.png)


# 🌍 Proyecto de Clasificación Binaria de Sismos en Tierra del Fuego

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)  
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)](https://scikit-learn.org/)  
[![Estado](https://img.shields.io/badge/estado-final-success)]()  
[![Licencia](https://img.shields.io/badge/licencia-MIT-blue)](LICENSE)

---

Este proyecto de **Machine Learning** tiene como objetivo desarrollar un modelo de aprendizaje automático que permita clasificar eventos sísmicos registrados en la región de Tierra del Fuego, Argentina, en dos categorías: **significativos** (percibidos o con impacto) y **no significativos**, a partir de características geográficas y técnicas.

## 📌 Objetivo General

El objetivo principal fue construir un modelo de clasificación binaria que permita predecir si un evento sísmico puede ser percibido por la población, combinando información geográfica y técnica del sismo.

La motivación detrás de este trabajo radica en la necesidad de anticipar eventos relevantes en una región con actividad sísmica baja pero con potencial de impacto. Un sistema así puede contribuir a mejorar la comunicación del riesgo y la planificación preventiva.

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
- 📂 Organización modular.

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

Se utilizó el Catálogo Sismológico de Referencia de Tierra del Fuego – Complemento 2021–2024, elaborado por:

Estación Astronómica Río Grande

Facultad de Ciencias Astronómicas y Geofísicas de la UNLP

CONICET

Red Sismológica Nacional de Chile

Este catálogo fue procesado con el software SEISAN v12.0, usando el algoritmo HYPOCENTER, reconocido internacionalmente para la localización de sismos.
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
- [📘 Ver reporte final del proyecto (PDF)](reports/Reporte_Clasificación_binaria_Tierra_del_Fuego.pdf)
- [🎞️ Ver presentación en PowerPoint (PDF)](reports/PowerPoint_del_proyecto.pdf)
- 🎥 [Ver video de presentación 1 (Abstract)](./Classifying%20earthquakes%20in%20Tierra%20del%20Fuego%20-%20Valeria%20Villegas.mp4)  
- 🎞️ [Ver video de presentación 2 (Proyecto completo)](./Proyecto%20Clasificación%20Binaria%20de%20Sismos%20en%20TDF%20-%20Valeria%20Villegas%20(1).mp4)

---

## 📈 Resultados destacados

- ✅ **Random Forest** es el mejor modelo: alta precisión, recall equilibrado, y ROC AUC > 0.9.
- 🧩 **Importancia de variables**: identificamos los factores más influyentes en la percepción de sismos.
- 📊 **Curvas ROC comparadas**: ofrecen una visual clara de la capacidad discriminativa de cada modelo para diferentes umbrales.
- 📉 **Matriz de confusión**: permite evaluar fallos de clasificación en cada clase.

---
✅ Conclusiones
El proyecto demostró que, aún con un dataset desbalanceado y limitado, es posible construir un modelo predictivo útil para anticipar eventos sísmicos percibidos.

Random Forest fue el modelo más eficaz, logrando un buen ROC AUC (0.861) y capacidad parcial para detectar la clase minoritaria.

El accuracy, por sí solo, no fue un buen indicador del desempeño, especialmente en este caso con clases desbalanceadas.

Este modelo puede tener un potencial aporte a la gestión del riesgo en regiones como Tierra del Fuego, donde los sismos no son frecuentes pero sí relevantes.

---
🚀 Trabajo Futuro
Algunas líneas de mejora y expansión del proyecto:

Aplicar técnicas de balanceo como SMOTE o ADASYN para mejorar la detección de eventos percibidos

Incluir nuevas variables como:

Tipo de suelo

Duración del evento

Densidad poblacional

Intensidad instrumental

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
