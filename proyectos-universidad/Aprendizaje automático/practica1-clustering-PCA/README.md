# ✈️ Predicción de la satisfacción de pasajeros - Proyecto grupal AA I

Este proyecto fue realizado como parte de la asignatura **Aprendizaje Automático I** del Grado en Ciencia e Ingeniería de Datos. El objetivo principal fue aplicar técnicas de reducción de dimensionalidad y aprendizaje no supervisado sobre un conjunto de datos reales de una necuesta de sstisfacción de clientes de una aerolínea.


📂 [Dataset original](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction)
---

## 🎯 Objetivos del proyecto

- Comprender el problema, cargar y explorar el dataset.
- Realizar un análisis exploratorio y preparación de los datos.
- Aplicar reducción de dimensionalidad mediante **PCA**, usando:
  - La función `prcomp()` de R.
  - Una implementación manual sin funciones específicas.
- Aplicar **clustering jerárquico y no jerárquico** sobre los datos.
- Evaluar distancias, desemejanzas y comprobar si cumplen condiciones de métrica.
- Extraer conclusiones y proponer líneas de trabajo futuras.

---

## 🛠 Herramientas utilizadas

- R
- R Markdown
- Librerías: `stats`, `cluster`, `factoextra`, `ggplot2`, `dplyr`

---

## 📂 Estructura de archivos
- R markdown
- html

---

## 📌 Notas adicionales

- Las variables usadas para PCA fueron: `Swim.Time`, `Bike.Time` y `Run.Time`.
- Se implementó una matriz de distancias personalizada y se validó su uso como métrica.
- Se aplicaron métodos de agrupamiento como K-means y jerárquico para comparar resultados.

---

## 👥 Integrantes del grupo

- Lorena Villa
- Lucía Arnaldo
- Álvaro Sánchez

---

## 📄 Licencia

Este proyecto está compartido como parte de mi portfolio académico y se encuentra bajo la licencia Apache 2.0.
