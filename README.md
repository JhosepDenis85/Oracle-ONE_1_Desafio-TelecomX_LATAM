# 📊 Análisis de Churn en TelecomX LATAM

> Proyecto de Análisis de Datos y Ciencia de Datos para identificar y predecir la evasión de clientes en una empresa de telecomunicaciones.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.0%2B-orange)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Compatible-yellow)

---

## 📋 Tabla de Contenidos

- [Descripción del Proyecto](#-descripción-del-proyecto)
- [Contexto del Problema](#-contexto-del-problema)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Requisitos y Dependencias](#-requisitos-y-dependencias)
- [Instalación](#-instalación)
- [Cómo Ejecutar el Proyecto](#-cómo-ejecutar-el-proyecto)
- [Descripción de las Secciones](#-descripción-de-las-secciones)
- [Resultados Esperados](#-resultados-esperados)
- [Problemas Comunes y Soluciones](#-problemas-comunes-y-soluciones)
- [Estructura de Datos](#-estructura-de-datos)
- [Contribución](#-contribución)
- [Licencia](#-licencia)

---

## 🎯 Descripción del Proyecto

Este proyecto implementa un **análisis exploratorio de datos (EDA)** completo para identificar patrones de evasión (churn) de clientes en TelecomX LATAM. El análisis incluye:

- ✅ Extracción de datos desde repositorio GitHub
- ✅ Transformación y limpieza de datos JSON anidados
- ✅ Análisis exploratorio con visualizaciones
- ✅ Identificación de factores de riesgo de churn
- ✅ Generación de insights accionables
- ✅ Informe final ejecutivo con recomendaciones estratégicas

---

## 🔍 Contexto del Problema

### El Desafío del Churn

**TelecomX LATAM** enfrenta un desafío crítico: aproximadamente el **25.7% de sus clientes abandonan el servicio** (churn). Esta evasión representa:

- 💸 Pérdida significativa de ingresos recurrentes
- 📉 Aumento de costos de adquisición de nuevos clientes (CAC)
- 🔻 Reducción del valor de vida del cliente (CLV)

### Objetivo del Análisis

Identificar **patrones y segmentos de alto riesgo** mediante análisis de datos para diseñar estrategias de retención efectivas que reduzcan la tasa de churn del 25.7% al ~18% en 12 meses.

---

## 📁 Estructura del Proyecto

```
Desafio 1/
│
├── TelecomX_LATAM_v9_Final.ipynb    # Notebook principal con análisis completo
├── TelecomX_Data.json               # Dataset (cargado desde GitHub)
├── TelecomX_diccionario.md          # Diccionario de datos
├── README.md                        # Este archivo
└── df_flat.xlsx                     # Exportación del DataFrame procesado (generado)
```

---

## 🛠️ Requisitos y Dependencias

### Requisitos del Sistema

- **Python**: 3.8 o superior
- **Entorno recomendado**: Google Colab (online, sin instalación) o Jupyter Notebook
- **Memoria RAM**: Mínimo 4GB
- **Conexión a Internet**: Necesaria para cargar datos desde GitHub

### Dependencias de Python

El proyecto utiliza las siguientes bibliotecas:

| Librería | Versión Mínima | Propósito |
|----------|----------------|-----------|
| `pandas` | 2.0+ | Manipulación y análisis de datos |
| `matplotlib` | 3.0+ | Visualización de datos |
| `openpyxl` | 3.0+ | Exportación a Excel (opcional) |

---

## 🚀 Instalación

### Opción 1: Google Colab (Recomendado - Sin instalación)

1. **Abrir el notebook directamente en Google Colab**:
   - Ve a [Google Colab](https://colab.research.google.com/)
   - Selecciona `Archivo > Abrir notebook`
   - Sube el archivo `TelecomX_LATAM_v9_Final.ipynb`

2. **Las dependencias ya están preinstaladas** en Colab (pandas, matplotlib)

3. **¡Listo para ejecutar!** 🎉

---

### Opción 2: Entorno Local (Jupyter Notebook)

#### Paso 1: Clonar o descargar el proyecto

```bash
# Si tienes Git instalado
git clone <url-del-repositorio>
cd "Desafio 1"

# O descarga el ZIP y extráelo
```

#### Paso 2: Crear entorno virtual (Recomendado)

```bash
# Windows PowerShell
python -m venv .venv
.\.venv\Scripts\Activate.ps1

# Windows CMD
python -m venv .venv
.venv\Scripts\activate.bat

# macOS/Linux
python3 -m venv .venv
source .venv/bin/activate
```

#### Paso 3: Instalar dependencias

```bash
pip install --upgrade pip
pip install pandas matplotlib openpyxl jupyter notebook
```

#### Paso 4: Iniciar Jupyter Notebook

```bash
jupyter notebook
```

Se abrirá automáticamente en tu navegador. Navega a `TelecomX_LATAM_v9_Final.ipynb` y ábrelo.

---

## ▶️ Cómo Ejecutar el Proyecto

### Ejecución Paso a Paso (Recomendado para aprendizaje)

1. **Abrir el notebook** en Google Colab o Jupyter
2. **Ejecutar las celdas secuencialmente** de arriba a abajo:
   - Usa `Shift + Enter` para ejecutar cada celda
   - Revisa los outputs de cada sección

### Ejecución Completa (Para resultados rápidos)

En Google Colab:
```
Menú → Entorno de ejecución → Ejecutar todas
```

En Jupyter Notebook:
```
Menú → Cell → Run All
```

### Tiempo de Ejecución Estimado

- ⏱️ **Ejecución completa**: 2-3 minutos
- ⏱️ **Carga de datos**: ~10 segundos
- ⏱️ **Visualizaciones**: ~30 segundos

---

## 📚 Descripción de las Secciones

El notebook está organizado en **15 secciones principales**:

### 1️⃣ Extracción de Datos
- **Objetivo**: Cargar dataset desde GitHub
- **Herramientas**: `pd.read_json()`
- **Output**: DataFrame con estructura JSON anidada

### 2️⃣ Transformación de Datos
- **Objetivo**: Convertir JSON anidado a tabla plana
- **Herramientas**: `pd.json_normalize()`
- **Output**: DataFrame con columnas aplanadas (ej: `customer.gender`, `account.Charges.Monthly`)

### 3️⃣ Comprobación de Datos
- **Objetivo**: Identificar y tratar valores nulos
- **Acciones**:
  - Detectar nulos con `.isnull().sum()`
  - Rellenar con `.fillna(0)`
  - Convertir tipos de datos con `pd.to_numeric()`

### 4️⃣ Ingeniería de Características
- **Objetivo**: Crear columnas calculadas
- **Columnas creadas**:
  - `Cuentas_Diarias`: Cargo total / días de antigüedad
  - `Cargo_Por_Mes`: Cargo total / meses de antigüedad
  - `Es_Cliente_Nuevo`: Antigüedad < 12 meses

### 5️⃣ Estandarización de Datos
- **Conversión de valores binarios**:
  - `Churn`: "Yes"/"No" → 1/0
  - `Partner`: "Yes"/"No" → 1/0
  - `Dependents`: "Yes"/"No" → 1/0
- **Traducción al español**:
  - `Gender`: "Male"/"Female" → "Masculino"/"Femenino"
  - `Contract`: "Month-to-month" → "Mes a mes"
  - `InternetService`: "Fiber optic" → "Fibra óptica"

### 6️⃣ Renombrado de Columnas
- **Objetivo**: Nombres descriptivos en español
- **Ejemplos**:
  - `customer.tenure` → `Meses_Cliente`
  - `account.Charges.Monthly` → `Cargo_Mensual`
  - `account.Charges.Total` → `Cargo_Total`

### 7️⃣ Análisis de Variables Numéricas
- Estadísticas descriptivas (mean, median, std, min, max)
- Variables analizadas:
  - Cargo Mensual
  - Cargo Total
  - Antigüedad del Cliente

### 8️⃣ Análisis de Variables Categóricas
- Distribución de frecuencias con `value_counts()`
- Variables analizadas:
  - Churn (variable objetivo)
  - Género
  - Servicio de Internet
  - Tipo de Contrato

### 9️⃣ Análisis Agrupado
- Análisis por segmentos usando `groupby()`
- Ejemplos:
  - Cargo promedio por tipo de contrato
  - Churn rate por género
  - Antigüedad promedio por servicio de internet

### 🔟 Análisis de Correlación
- Relaciones entre variables usando `pd.crosstab()`
- Identificación de factores de riesgo

### 1️⃣1️⃣ Reto 6: Distribución de Evasión
- **Visualizaciones**:
  - Gráfico de barras: Conteo de clientes por estado de churn
  - Gráfico circular (pie chart): Proporción de churn

### 1️⃣2️⃣ Reto 7: Recuento por Variables Categóricas
- **Análisis de churn por**:
  - Género
  - Tipo de Contrato
  - Servicio de Internet
  - Método de Pago
- **Visualizaciones**: Tablas de contingencia + gráficos de barras

### 1️⃣3️⃣ Reto 8: Conteo por Variables Numéricas
- **Análisis de churn según**:
  - Cargo Total (histogramas + boxplots)
  - Cargo Mensual (boxplots)
  - Antigüedad del Cliente (histogramas + boxplots)
- **Visualización final**: Comparación de medias

### 1️⃣4️⃣ Informe Final
Documento ejecutivo con:
- 📌 **Introducción**: Contexto y objetivos
- 🔧 **Limpieza de Datos**: Metodología aplicada
- 📊 **Análisis Exploratorio**: Hallazgos principales
- 💡 **Conclusiones**: 4 factores de riesgo identificados
- 🎯 **Recomendaciones**: 6 estrategias con KPIs específicos

---

## 📈 Resultados Esperados

Al ejecutar el notebook completo, obtendrás:

### Outputs Visuales
- ✅ **21 visualizaciones** (gráficos de barras, circulares, histogramas, boxplots)
- ✅ **Tablas de estadísticas descriptivas** para variables numéricas
- ✅ **Tablas de contingencia** para análisis categórico

### Insights Clave Identificados

| Hallazgo | Métrica |
|----------|---------|
| Tasa de churn global | **25.7%** |
| Mayor riesgo: Contratos mes a mes | Churn ~42% |
| Mayor riesgo: Pago con electronic check | Churn ~45% |
| Mayor riesgo: Cargo mensual alto | Media $91 vs $61 |
| Mayor riesgo: Baja antigüedad | Media 18 meses vs 37 meses |

### Archivo Exportado
- `df_flat.xlsx`: DataFrame procesado (opcional)

---

## ⚠️ Problemas Comunes y Soluciones

### Problema 1: Error al cargar datos desde GitHub

**Error**:
```
URLError: <urlopen error [SSL: CERTIFICATE_VERIFY_FAILED]>
```

**Solución**:
```python
# Agregar al inicio del notebook
import ssl
ssl._create_default_https_context = ssl._create_unverified_context
```

---

### Problema 2: ValueError en gráfico circular (pie chart)

**Error**:
```
ValueError: 'explode' must be of length 'x', not 2
```

**Solución** (YA CORREGIDA en v9_Final):
```python
# Usar explode dinámico
explode = tuple([0.05] * len(churn_counts))
plt.pie(churn_counts, explode=explode, ...)
```

---

### Problema 3: Columnas no encontradas después de renombrado

**Error**:
```
KeyError: 'Cargo_Mensual'
```

**Solución**:
```python
# Usar condicional para detectar nombre de columna
col_mensual = 'Cargo_Mensual' if 'Cargo_Mensual' in df_flat.columns else 'account.Charges.Monthly'
df_flat[col_mensual].mean()
```

---

### Problema 4: Gráficos no se visualizan en Jupyter

**Solución**:
```python
# Agregar al inicio del notebook
%matplotlib inline
import matplotlib.pyplot as plt
```

---

### Problema 5: Error de memoria al exportar Excel

**Error**:
```
MemoryError
```

**Solución**:
```python
# Exportar solo columnas necesarias
df_flat[['customerID', 'Churn', 'Cargo_Mensual']].to_excel('df_flat_lite.xlsx')

# O exportar a CSV (más eficiente)
df_flat.to_csv('df_flat.csv', index=False)
```

---

### Problema 6: Versión de pandas incompatible

**Error**:
```
AttributeError: 'DataFrame' object has no attribute 'append'
```

**Solución**:
```bash
# Actualizar pandas
pip install --upgrade pandas

# O usar concat en lugar de append
pd.concat([df1, df2], ignore_index=True)
```

---

## 🗂️ Estructura de Datos

### Dataset Original (JSON)

El dataset se carga desde:
```
https://raw.githubusercontent.com/ingridcristh/challenge2-data-science-LATAM/main/TelecomX_Data.json
```

**Estructura JSON anidada**:
```json
{
  "customerID": "7590-VHVEG",
  "Churn": "No",
  "customer": {
    "gender": "Female",
    "SeniorCitizen": 0,
    "Partner": "Yes",
    "Dependents": "No"
  },
  "account": {
    "tenure": 1,
    "Contract": "Month-to-month",
    "PaymentMethod": "Electronic check",
    "Charges": {
      "Monthly": 29.85,
      "Total": "29.85"
    }
  },
  "internet": {
    "InternetService": "DSL",
    "OnlineSecurity": "No",
    "StreamingTV": "No"
  }
}
```

### Dimensiones del Dataset

- **Filas**: 7,267 clientes
- **Columnas después de aplanar**: ~21 columnas
- **Variable objetivo**: `Churn` (Yes/No)

### Variables Principales

| Nombre Original | Nombre Español | Tipo | Descripción |
|----------------|----------------|------|-------------|
| `customerID` | ID_Cliente | string | Identificador único |
| `Churn` | Evasión | binario | Yes=1, No=0 |
| `customer.gender` | Genero | categórico | Masculino/Femenino |
| `customer.SeniorCitizen` | Es_Adulto_Mayor | binario | 1=Sí, 0=No |
| `account.tenure` | Meses_Cliente | numérico | Antigüedad en meses |
| `account.Contract` | Tipo_Contrato | categórico | Mes a mes / Un año / Dos años |
| `account.Charges.Monthly` | Cargo_Mensual | numérico | Cargo mensual en USD |
| `account.Charges.Total` | Cargo_Total | numérico | Cargo total acumulado |
| `account.PaymentMethod` | Metodo_Pago | categórico | Forma de pago |
| `internet.InternetService` | Servicio_Internet | categórico | DSL / Fibra / Sin servicio |

---

## 📊 Visualizaciones Incluidas

El notebook genera las siguientes visualizaciones:

### Reto 6 (3 gráficos)
1. Gráfico de barras de distribución de churn
2. Gráfico circular de proporción de churn

### Reto 7 (8 gráficos)
3. Churn por género (tabla + gráfico)
4. Churn por tipo de contrato (tabla + gráfico de barras apiladas)
5. Churn por servicio de internet (tabla + gráfico)
6. Churn por método de pago (tabla + gráfico horizontal)

### Reto 8 (10 gráficos)
7. Estadísticas de cargo total por churn
8. Histograma de cargo total
9. Boxplot de cargo total
10. Boxplot de cargo mensual
11. Estadísticas de antigüedad
12. Histograma de antigüedad
13. Boxplot de antigüedad
14. Comparación de medias (3 variables)

### Informe Final (2 gráficos)
15. Visualización resumen de distribución general
16. Comparación de medias de variables numéricas

**Total: 21+ visualizaciones**

---

## 🎓 Habilidades Demostradas

Este proyecto demuestra competencias en:

- ✅ **Extracción de datos** desde APIs/GitHub
- ✅ **Transformación de datos** (JSON anidado → tabla plana)
- ✅ **Limpieza de datos** (nulos, tipos, outliers)
- ✅ **Ingeniería de características** (feature engineering)
- ✅ **Análisis exploratorio de datos** (EDA)
- ✅ **Visualización de datos** con matplotlib
- ✅ **Análisis estadístico descriptivo**
- ✅ **Interpretación de resultados** y generación de insights
- ✅ **Comunicación técnica** (informe ejecutivo)
- ✅ **Pensamiento analítico** orientado a negocio

---

## 🤝 Contribución

Si deseas contribuir a este proyecto:

1. **Fork** el repositorio
2. Crea una **rama** para tu feature (`git checkout -b feature/AmazingFeature`)
3. **Commit** tus cambios (`git commit -m 'Add: AmazingFeature'`)
4. **Push** a la rama (`git push origin feature/AmazingFeature`)
5. Abre un **Pull Request**

---

## 📧 Contacto

**Proyecto desarrollado por**: Equipo de Ciencia de Datos TelecomX  
**Fecha de creación**: Febrero 2026  
**Versión**: v9 Final  

---

## 📄 Licencia

Este proyecto es de código abierto y está disponible bajo la licencia MIT.

---

## 🔖 Notas Adicionales

### Próximos Pasos (Roadmap)

- [ ] Implementar modelo predictivo de churn con Machine Learning
- [ ] Desarrollar dashboard interactivo con Plotly/Dash
- [ ] Análisis de series temporales (evolución del churn)
- [ ] Segmentación de clientes con clustering (K-means)
- [ ] Optimización de hiperparámetros con GridSearchCV
- [ ] Implementación de API REST para predicciones

### Recursos Adicionales

- 📖 [Documentación de Pandas](https://pandas.pydata.org/docs/)
- 📖 [Documentación de Matplotlib](https://matplotlib.org/stable/contents.html)
- 📖 [Google Colab FAQ](https://research.google.com/colaboratory/faq.html)
- 📖 [Diccionario de Datos](TelecomX_diccionario.md)

---

<div align="center">

**⭐ Si este proyecto te fue útil, no olvides darle una estrella ⭐**

**Hecho con ❤️ por el equipo de Data Science**

</div>
