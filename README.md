# 📊 Análisis de Agrupamiento en Datos de la Competición DE mediante Algoritmos de Clustering

## 📌 Descripción  
Este proyecto evalúa diversos algoritmos de **aprendizaje no supervisado** para identificar agrupamientos en los datos de la competición DE. Para ello se han cogido los datos provenientes de la competición: https://www.drivendata.org/competitions/44/dengai-predicting-disease-spread/. El archivo es *dengue_features_train.csv*.

La metodología se divide en dos fases:

1. **Exploración y selección de características**: Se realiza un análisis estadístico del conjunto de datos y se imputan valores nulos mediante técnicas iterativas. La selección de características se basa en **K-Means** y **clustering jerárquico**.
2. **Aplicación de algoritmos de clustering**: Se implementan cuatro métodos de agrupamiento, incluyendo uno no estudiado en clase. Para visualizar los resultados, se utilizan técnicas de **reducción de dimensionalidad**.

Tras la evaluación, **DBSCAN obtuvo los peores resultados**, mientras que los demás generaron agrupamientos similares. La selección del mejor modelo se detalla en las conclusiones.

---

## 🛠️ Tecnologías Utilizadas  

### 📌 Lenguaje de Programación  
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

### 📌 Librerías Principales  
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white) ![Scikit-Learn](https://img.shields.io/badge/Scikit%20Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=plotly&logoColor=white) ![Seaborn](https://img.shields.io/badge/Seaborn-008080?style=for-the-badge&logo=python&logoColor=white)

---

## 📂 Estructura del Proyecto  

📄 models.ipynb → Notebook que contiene todo el desarrollo del proyecto

---

## 🚀 Algoritmos Implementados  
✔ **K-Means** → Algoritmo de clustering basado en centroides.  
✔ **Clustering Jerárquico Aglomerativo** → Algoritmo basado en fusiones sucesivas.  
✔ **DBSCAN** → Algoritmo basado en densidad.  
✔ **Spectral Clustering** → Algoritmo basado en grafos y transformaciones espectrales.  

---

## 📈 Resultados y Conclusiones  
Este proyecto evaluó cuatro algoritmos de clustering con las mismas características: **station_diur_temp_rng_c**, **station_avg_temp_c**, **precipitation_amt_mm**, **station_precip_mm** y **reanalysis_relative_humidity_percent**.

- **DBSCAN** obtuvo los peores resultados debido a la métrica de distancia o la distribución de los datos.
- **K-Means** mostró un buen rendimiento pero con una distribución desigual de puntos y poca tolerancia al ruido.
- **Clustering Jerárquico Aglomerativo** tuvo un rendimiento bajo y escasa tolerancia al ruido.
- **Spectral Clustering** presentó la mejor distribución de puntos y mayor tolerancia al ruido, aunque con rendimiento inferior.

Dado que la menor pérdida de rendimiento no afecta debido al tamaño del dataset, **Spectral Clustering** es la mejor opción, pero se recomienda un análisis más detallado sobre el número óptimo de clusters. El proyecto fue una experiencia didáctica valiosa para aplicar técnicas de clustering.


