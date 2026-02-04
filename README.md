# 🏘️ Predictive Real Estate Valuation: Monterrey Case Study

Este proyecto desarrolla un modelo de **Data Science** y **Análisis Espacial** para estimar el precio por metro cuadrado ($m^2$) de desarrollos residenciales en Monterrey, México. El objetivo es proporcionar una herramienta de **Foresight Inmobiliario** que sustente la toma de decisiones basada en datos de mercado y variables geográficas.

---

## 🚀 Objetivo del Proyecto
Determinar el valor comercial de un terreno o proyecto inmobiliario considerando no solo sus atributos físicos (amenidades), sino su contexto urbano y proximidad a nodos de valor económico mediante el uso de **PostGIS** y **Machine Learning**.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python 3.x
* **Análisis Geospacial:** GeoPandas, Shapely, PyProj.
* **Base de Datos:** PostgreSQL + PostGIS (SQL Avanzado).
* **Machine Learning:** Scikit-Learn (Random Forest Regressor).
* **Visualización:** Folium (Mapas interactivos) y Seaborn/Matplotlib.

---

## 📊 Metodología
1. **Extracción y Limpieza:** Procesamiento de datos de competencia inmobiliaria (precios, ubicaciones, amenidades).
2. **Ingeniería de Variables (GIS):** * Transformación de coordenadas (EPSG:4326 a EPSG:32614).
    * Cálculo de distancias euclidianas a Nodos de Valor (Distrito de Negocios San Pedro).
3. **Modelado:** Entrenamiento de un **Random Forest Regressor** para capturar relaciones no lineales entre la ubicación y el precio.
4. **Validación:** Evaluación mediante Error Medio Absoluto (MAE) para garantizar la utilidad del modelo en el mundo real.

---

## 📈 Análisis de Resultados: Feature Importance
Uno de los mayores aportes de este modelo es la capacidad de explicar **qué factores mueven el precio** en la zona de estudio. Según nuestro análisis de importancia de variables:



* **Distancia al Nodo de Valor (65%):** Es el factor determinante. La cercanía a centros de empleo y servicios de lujo en San Pedro Garza García impacta exponencialmente el precio.
* **Número de Amenidades (25%):** El mercado valora significativamente la oferta de áreas comunes (albercas, gimnasios, coworkings), permitiendo un "premium" sobre el precio base.
* **Otros factores (10%):** Variables secundarias y ruido de mercado.

> **Insight para Consultoría:** Un desarrollador puede justificar un aumento en el precio de venta si invierte en amenidades específicas, incluso si el terreno no se encuentra en el "punto cero" del nodo de valor.

---

## 🗺️ Visualización Interactiva
El proyecto incluye un mapa generado con **Folium** que permite visualizar la "temperatura" de los precios en la zona y la ubicación estratégica de la competencia frente al nodo de valor.

---
**Contacto:** Eliuth Rojas - https://www.linkedin.com/in/eliuthrojas/
