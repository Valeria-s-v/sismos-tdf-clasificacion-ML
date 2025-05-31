
# 📊 Descripción del Dataset Sísmico

## 📁 Fuente y Origen
- **Institución**: Instituto Nacional de Prevención Sísmica (INPRES)
- **Período cubierto**: Enero 2021 – Abril 2024
- **Región geográfica**: Provincia de Tierra del Fuego, Argentina
- **Método de adquisición**: Extracción de tablas desde PDF oficial del catálogo sísmico mediante `tabula-py`.
- **Licencia**: Datos públicos de uso académico.

## 📦 Estructura del Dataset
- **Cantidad de registros (filas)**: 332
- **Cantidad de columnas (atributos)**: 18

### 🧬 Principales columnas:
| Columna                | Descripción                                              | Tipo de dato |
|------------------------|----------------------------------------------------------|--------------|
| `anio`, `mes`, `dia`   | Fecha de ocurrencia del evento                           | Entero       |
| `hora`, `minuto`, `segundo` | Hora exacta del evento                         | Entero/Decimal |
| `latitud`, `longitud`  | Coordenadas geográficas del epicentro                    | Float        |
| `profundidad_km`       | Profundidad del sismo en kilómetros                      | Float        |
| `magnitud_ml`          | Magnitud local del evento (escala ML)                    | Float        |
| `clasificacion_distancia` | Tipo de evento según cercanía o región              | Categórica   |
| `dist_*`               | Distancia desde el epicentro a ciudades claves (km)      | Float        |
| `ciudad_mas_cercana`   | Determinación automática de la ciudad más próxima        | Categórica   |
| `significativo`        | Variable binaria objetivo: 1 = percibido / 0 = no        | Binaria      |

## ⚙️ Preprocesamiento Realizado
- Limpieza de valores nulos
- Conversión de comas decimales a puntos
- Conversión de tipos de datos
- Cálculo de distancias geográficas a tres ciudades principales
- Generación de la variable `significativo` (basada en ML y cercanía)

## 🧠 Tipo de problema
- Clasificación supervisada binaria

## ✅ Estado del Dataset
- Listo para análisis exploratorio y modelado con algoritmos de machine learning.
