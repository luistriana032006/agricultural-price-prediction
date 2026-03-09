# 🌱 Agricultural Price Prediction — Santander, Colombia

> Modelo de predicción de precios agrícolas para pequeños productores de cacao y café en Santander, Colombia.  
> Proyecto desarrollado en el marco del programa **GCI World — Matsuo-Iwasawa Laboratory, Universidad de Tokyo (2026)**.

---

## 🎯 Objetivo

Construir una herramienta de soporte a la decisión para **cacaoteros y cafeteros** de los municipios de San Gil y Socorro (Santander), que les permita anticipar variaciones en los precios de sus productos usando datos históricos, climáticos y económicos.

Santander es el **mayor productor de cacao de Colombia** — este proyecto nace de la necesidad real de los agricultores de la región de tomar mejores decisiones de venta y producción.

---

## 📊 Datos

| Fuente | Variable | Frecuencia |
|--------|----------|------------|
| SIPSA / DANE | Precios mayoristas en Bucaramanga | Diaria |
| Agronet | Producción agrícola Santander | Mensual |
| Fedecacao | Precios y producción de cacao | Mensual |
| Fedecafé API | Precios internos del café | Diaria |
| IDEAM | Variables climáticas (temperatura, precipitación) | Diaria |
| Banco de la República | Tasa de cambio USD/COP | Diaria |
| datos.gov.co | Datos abiertos agropecuarios Colombia | Variable |
| Google Trends | Demanda proxy por producto | Semanal |

Rango temporal objetivo: **2022 – 2025** (3 años de historia)

---

## 🧠 Metodología

```
Recolección de datos → Limpieza y unificación → Análisis exploratorio (EDA)
        ↓
Feature engineering (variables lag, clima, estacionalidad)
        ↓
Modelos baseline (ARIMA, Prophet)
        ↓
Modelos avanzados (XGBoost, LSTM)
        ↓
Evaluación (MAE, RMSE, MAPE)
        ↓
Despliegue como herramienta de consulta
```

---

## 🛠️ Stack Técnico

- **Lenguaje:** Python 3.11+
- **Análisis de datos:** Pandas, NumPy
- **Visualización:** Matplotlib, Seaborn, Plotly
- **Modelos ML:** Scikit-learn, XGBoost
- **Series de tiempo:** Statsmodels (ARIMA), Prophet
- **Deep Learning:** TensorFlow / Keras (LSTM)
- **Notebooks:** Jupyter
- **Control de versiones:** Git / GitHub

---

## 📁 Estructura del Proyecto

```
agricultural-price-prediction/
│
├── data/
│   ├── raw/              # Datos originales sin procesar
│   ├── processed/        # Datos limpios y unificados
│   └── external/         # Datos de fuentes externas
│
├── notebooks/
│   ├── 01_eda.ipynb              # Análisis exploratorio
│   ├── 02_feature_engineering.ipynb
│   ├── 03_baseline_models.ipynb
│   └── 04_advanced_models.ipynb
│
├── src/
│   ├── data/             # Scripts de recolección y limpieza
│   ├── features/         # Feature engineering
│   └── models/           # Entrenamiento y evaluación
│
├── reports/
│   └── figures/          # Gráficas y visualizaciones
│
├── requirements.txt
└── README.md
```

---

## 🚧 Estado del Proyecto

| Fase | Estado |
|------|--------|
| Definición del problema | ✅ Completado |
| Identificación de fuentes de datos | ✅ Completado |
| Recolección de datos | 🔄 En progreso |
| Limpieza y EDA | ⏳ Pendiente |
| Modelos baseline | ⏳ Pendiente |
| Modelos avanzados | ⏳ Pendiente |
| Despliegue | ⏳ Pendiente |

---

## 🌍 Contexto

Este proyecto hace parte del programa **GCI World** organizado por el **Matsuo-Iwasawa Laboratory** de la **Universidad de Tokyo**, que reúne estudiantes de todo el mundo para trabajar en proyectos de IA aplicada a problemas reales.

El enfoque está en el impacto social: los pequeños agricultores de Santander no tienen acceso a herramientas de análisis de mercado. Este modelo busca cerrar esa brecha usando datos abiertos y machine learning.

---

## 👨‍💻 Autor

**Luis Miguel Triana Rueda**  
ML Engineering Student · Backend Developer  
Socorro, Santander, Colombia → Dubai 2027

- 🌐 Portfolio: [luistriana.vercel.app](https://luistriana.vercel.app)
- 💼 LinkedIn: [linkedin.com/in/luismigueltr](https://www.linkedin.com/in/luis-triana-2917202a2/)
- 🐙 GitHub: [github.com/luistriana032006](https://github.com/luistriana032006)

---

*"De Socorro, Santander — hacia el mundo."*
