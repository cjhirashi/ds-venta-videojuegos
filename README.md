# 🎮 Análisis de Ventas de Videojuegos

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green?logo=pandas)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?logo=plotly)](https://matplotlib.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)

---

## 🚀 Descripción

Este proyecto corresponde al **Sprint 6** del programa de Ciencia de Datos en **TripleTen**.
El objetivo es analizar datos de ventas de videojuegos a nivel global, identificar patrones de éxito y probar hipótesis estadísticas que permitan apoyar decisiones estratégicas en campañas de marketing y selección de plataformas.

El caso práctico se basa en datos históricos hasta 2016, con el propósito de planear una estrategia de ventas para 2017.

Accesa al Notebook: [/notebook/sprint6_analysis.ipynb](https://github.com/cjhirashi/proyecto-sprint-6/blob/main/notebooks/sprint6_analysis.ipynb)

---

## ✨ Objetivos principales

* Preparar y limpiar los datos 📊
* Identificar plataformas y géneros con mayor potencial de éxito 🎮
* Analizar la relación entre reseñas (usuarios y críticos) y ventas ⭐
* Construir perfiles de usuario para distintas regiones (NA, EU, JP) 🌎
* Probar hipótesis estadísticas sobre plataformas y géneros 📈

---

## 🧰 Tecnologías utilizadas

* [Python 3](https://www.python.org/)
* [Pandas](https://pandas.pydata.org/)
* [NumPy](https://numpy.org/)
* [Matplotlib](https://matplotlib.org/)
* [Seaborn](https://seaborn.pydata.org/)
* [Jupyter Notebook](https://jupyter.org/)
* [Pipenv](https://pipenv.pypa.io/en/latest/) – gestión de entornos y dependencias

---

## ⚙️ Estructura del proyecto

```bash
.
├── data/
│   └── games.csv          # Dataset principal de videojuegos
├── notebooks/
│   └── sprint6_analysis.ipynb   # Notebook con todo el análisis
├── Pipfile
├── Pipfile.lock
└── README.md
```

---

## ▶️ Instalación y uso

1. **Clonar repositorio**

   ```bash
   git clone https://github.com/cjhirashi/proyecto-sprint-6.git
   cd proyecto-sprint-6
   ```

2. **Crear entorno e instalar dependencias**

   ```bash
   pipenv install
   pipenv shell
   ```

---

## 📑 Dataset

**Archivo:** `/datasets/games.csv`

**Columnas principales:**

* `name` → Nombre del videojuego
* `platform` → Consola / Plataforma
* `year_of_release` → Año de lanzamiento
* `genre` → Género
* `na_sales`, `eu_sales`, `jp_sales`, `other_sales` → Ventas por región (millones USD)
* `critic_score` → Calificación de críticos (0–100)
* `user_score` → Calificación de usuarios (0–10)
* `rating` → Clasificación ESRB

---

## 📊 Resultados esperados

* Identificación de plataformas y géneros con mayor potencial de éxito.
* Distribuciones de ventas por región (NA, EU, JP) con perfiles de usuario.
* Correlación entre reseñas (usuarios y críticos) y ventas.
* Evaluación de hipótesis estadísticas en plataformas y géneros.
* Conclusiones estratégicas para orientar campañas de marketing.

---

## ✅ Conclusiones

El análisis de los datos de ventas de videojuegos (2013–2016) permitió identificar hallazgos clave:

1. **Tendencias globales**  
   - Picos de lanzamientos en 2008–2009, caída progresiva hacia 2016.  
   - *PS2*, *X360* y *PS3* fueron históricamente líderes; *PS4* tomó el liderazgo reciente.  
   - *Action* fue el género más rentable, seguido de *Shooter* y *Sports*.  

2. **Impacto de reseñas**  
   - Correlación moderada entre `critic_score` y ventas (ej. *PS4*).  
   - Correlación débil o negativa entre `user_score` y ventas, mostrando bajo poder predictivo.  

3. **Diferencias regionales**  
   - **NA/EU**: preferencias en *PS4/XOne* y géneros *Action/Shooter*.  
   - **JP**: fuerte preferencia por *Role-Playing* y consolas portátiles (*3DS*, *PSV*).  
   - El impacto de las clasificaciones ESRB es relevante en NA/EU, pero poco en JP.  

4. **Pruebas de hipótesis**  
   - No se detectaron diferencias significativas en calificaciones de usuario entre *Xbox One* y *PC*.  
   - Sí hubo diferencia significativa en ventas entre *Action* y *Sports*:  
     - Muestras: *Action* = 766 juegos, *Sports* = 214 juegos  
     - T-statistic = -2.991, p-valor = 0.003 (< 0.05)  
     - **Conclusión:** *Action* tiene un desempeño comercial significativamente superior a *Sports*.  

---

## 📌 Recomendaciones

- **Campañas regionales diferenciadas:**  
  - **NA/EU:** priorizar *Action*, *Shooter* y *Sports* en *PS4/XOne*.  
  - **JP:** promover *Role-Playing* en plataformas portátiles.  

- **Toma de decisiones:**  
  - Dar más peso a las reseñas de críticos para prever desempeño comercial.  
  - Usar reseñas de usuarios como insumo cualitativo más que predictor de ventas.  

- **Estrategia de inversión:**  
  - Apostar por géneros con crecimiento sostenido (*Action*, *Shooter*).  
  - Evitar grandes inversiones en géneros de bajo retorno como *Puzzle* o *Strategy*, salvo en nichos.  

---

## 👨‍💻 Autor

**Carlos Jiménez Hirashi**
💼 Data Scientist Jr. | Python & Machine Learning

📧 [cjhirashi@gmail.com](mailto:cjhirashi@gmail.com) · 🌐 [LinkedIn](https://www.linkedin.com/in/cjhirashi)
