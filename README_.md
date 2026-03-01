# 📊 Desafío Alura Store - Análisis de Datos con Python

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.0%2B-orange)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Compatible-yellow)
![Status](https://img.shields.io/badge/Status-Completo-success)

> **Análisis exhaustivo de 4 tiendas de comercio electrónico con más de 8,599 transacciones para determinar la estrategia óptima de desinversión del Sr. Juan.**

---

## 🎯 Descripción del Proyecto Desafío Alura Store

Este proyecto forma parte del programa **Oracle ONE (Oracle Next Education)** en colaboración con **Alura Latam**, y consiste en un análisis completo de datos de ventas de 4 tiendas de comercio electrónico para apoyar la decisión estratégica del Sr. Juan sobre **cuál tienda debe vender**.

### Contexto del Problema

El Sr. Juan posee 4 tiendas de comercio electrónico y necesita decidir estratégicamente cuál vender para optimizar su portafolio de negocios. Para tomar esta decisión, requiere un análisis exhaustivo basado en datos que considere:

- 💰 **Desempeño financiero**: Ingresos totales por tienda
- 📦 **Portafolio de productos**: Categorías más y menos vendidas
- ⭐ **Satisfacción del cliente**: Calificaciones promedio
- 🚚 **Eficiencia operativa**: Costos de envío
- 🌍 **Cobertura geográfica**: Distribución de ventas por ubicación
- 📊 **Análisis multidimensional**: Visualizaciones avanzadas

### Objetivo Principal

**Proporcionar una recomendación fundamentada en datos sobre qué tienda vender**, respaldada por análisis cuantitativo, visualizaciones profesionales y un informe ejecutivo completo.

---

## 📐 Estructura del Análisis

El proyecto está organizado en **7 secciones** más un **informe final**:

```
Sección 1: Análisis de Facturación
    ├── Cálculo de ingresos totales
    └── Visualización comparativa

Sección 2: Ventas por Categoría
    ├── Distribución de productos por categoría
    └── Gráficos de barras horizontales 4-panel

Sección 3: Calificación Promedio
    ├── Satisfacción del cliente por tienda
    └── Comparativa con línea de referencia

Sección 4: Productos Más y Menos Vendidos
    ├── Identificación de productos estrella
    └── Top 10 productos por tienda

Sección 5: Envío Promedio por Tienda
    ├── Análisis de eficiencia logística
    ├── Resumen comparativo consolidado
    └── Dashboard 4-panel de métricas clave

Sección 6: Generando Gráficos Avanzados
    ├── Scatter plot: Precio vs Calificación
    ├── Pie chart: Distribución de categorías
    ├── Boxplot: Distribución de precios
    ├── Histogram: Distribución de calificaciones
    ├── Line chart: Métricas normalizadas
    └── Stacked bar: Composición de ingresos

Sección 7: Análisis Geográfico
    ├── Exploración de coordenadas lat/lon
    ├── Mapas de dispersión por tienda
    ├── Heatmaps de concentración de ventas
    ├── Análisis por ciudad (Top 5)
    ├── Mapa consolidado de 4 tiendas
    └── Conclusiones geográficas

Informe Final
    ├── Introducción y metodología
    ├── Desarrollo del análisis (7 Secciones)
    ├── Matriz de puntuación ponderada
    ├── Análisis FODA por tienda
    ├── Conclusiones y recomendación
    └── Visualización final consolidada
```

---

## 🛠️ Requisitos y Dependencias

### Requisitos del Sistema

- **Python**: 3.8 o superior
- **Entorno recomendado**: Google Colab (online, sin instalación local)


### Dependencias de Python

El proyecto utiliza las siguientes bibliotecas estándar:

| Librería | Versión Mínima | Propósito |
|----------|----------------|-----------|
| `pandas` | 2.0+ | Manipulación y análisis de DataFrames |
| `matplotlib.pyplot` | 3.0+ | Visualización de datos (gráficos) |
| `numpy` | 1.21+ | Operaciones numéricas y arrays |

**Nota**: Estas bibliotecas están **preinstaladas en Google Colab**, por lo que no requieren instalación adicional.

---

## 🚀 Instalación

### Opción 1: Google Colab (Recomendado - Sin instalación)

1. **Abrir el notebook directamente en Google Colab**:
   - Ve a [Google Colab](https://colab.research.google.com/)
   - Selecciona `Archivo > Abrir notebook`
   - Sube el archivo `AluraStoreLatam_F.ipynb`

2. **Las dependencias ya están preinstaladas** en Colab (pandas, matplotlib, numpy)

3. **¡Listo para ejecutar!** 🎉

---

### Opción 2: Entorno Local (Jupyter Notebook)

#### Paso 1: Clonar o descargar el proyecto

```bash
# Si tienes Git instalado
git clone <url-del-repositorio>
cd Oracle-ONE_1_Desafio-Alura-Store_-Latam

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
pip install pandas matplotlib numpy jupyter notebook
```

#### Paso 4: Iniciar Jupyter Notebook

```bash
jupyter notebook
```

Se abrirá automáticamente en tu navegador. Navega a `AluraStoreLatam_F.ipynb` y ábrelo.

---

## ▶️ Cómo Ejecutar el Proyecto

### Ejecución Paso a Paso (Recomendado para aprendizaje)

1. **Abrir el notebook** en Google Colab o Jupyter
2. **Ejecutar las celdas secuencialmente** de arriba a abajo:
   - Usa `Shift + Enter` para ejecutar cada celda
   - Revisa los outputs de cada sección
   - Los gráficos se mostrarán automáticamente

**⚠️ IMPORTANTE**: Las variables se definen progresivamente. Ejecutar las celdas fuera de orden causará errores.

---

### Ejecución Completa (Para resultados rápidos)

En Google Colab:
```
Menú → Entorno de ejecución → Ejecutar todas
```

En Jupyter Notebook:
```
Menú → Cell → Run All
```

**Tiempo estimado de ejecución**: 2-3 minutos (dependiendo de la conexión a internet)

---

## 📚 Secciones Implementados

### 1️⃣ Sección 1: Análisis de Facturación

**Objetivo**: Calcular y comparar los ingresos totales de cada tienda

**Métodos utilizados**:
- `pandas.DataFrame.sum()` - Suma de columna 'Precio'
- `matplotlib.pyplot.bar()` - Gráfico de barras

**Output**:
- Ingresos totales por tienda (4 valores)
- Gráfico de barras comparativo con etiquetas

**Insight clave**: Tienda 1 genera los mayores ingresos

---

### 2️⃣ Sección 2: Ventas por Categoría

**Objetivo**: Analizar la distribución de productos vendidos por categoría

**Métodos utilizados**:
- `pandas.Series.value_counts()` - Conteo por categoría
- `matplotlib.pyplot.subplots()` - Grid de 4 gráficos

**Output**:
- Conteo de ventas por categoría (8 categorías aprox.)
- 4 gráficos de barras horizontales (uno por tienda)

**Insight clave**: Electrónicos y Muebles dominan las ventas

---

### 3️⃣ Sección 3: Calificación Promedio

**Objetivo**: Evaluar la satisfacción del cliente por tienda

**Métodos utilizados**:
- `pandas.Series.mean()` - Calificación promedio
- `matplotlib.pyplot.axhline()` - Línea de referencia

**Output**:
- Calificación promedio por tienda (escala 1-5)
- Gráfico con línea de referencia en 4.0

**Insight clave**: Todas las tiendas están por debajo del estándar (< 4.0)

---

### 4️⃣ Sección 4: Productos Más y Menos Vendidos

**Objetivo**: Identificar productos estrella y de baja rotación

**Métodos utilizados**:
- `pandas.Series.value_counts()` - Ranking de productos
- `.head()` y `.tail()` - Top y bottom productos

**Output**:
- Producto más vendido y menos vendido por tienda
- Top 10 productos en gráficos de 4 paneles

**Insight clave**: Alta concentración en productos estrella (Pareto)

---

### 5️⃣ Sección 5: Envío Promedio por Tienda

**Objetivo**: Analizar la eficiencia logística

**Métodos utilizados**:
- `pandas.Series.mean()` - Costo promedio de envío
- `pandas.DataFrame()` - Tabla resumen consolidada

**Output**:
- Costo de envío promedio por tienda
- Tabla resumen con 4 métricas clave
- Dashboard 4-panel comparativo

**Insight clave**: Tienda 2 tiene la logística más eficiente

---

### 6️⃣ Sección 6: Generando Gráficos Avanzados

**Objetivo**: Crear visualizaciones profesionales de múltiples tipos

**Métodos utilizados**:
- `plt.scatter()` - Gráfico de dispersión
- `plt.pie()` - Gráfico circular
- `plt.boxplot()` - Diagrama de caja y bigotes
- `plt.hist()` - Histograma
- `plt.plot()` - Gráfico de líneas
- Normalización 0-100 para comparación

**Output**:
- 6 tipos diferentes de visualizaciones
- Análisis de correlación precio-calificación
- Distribución de categorías
- Dispersión de precios
- Frecuencia de calificaciones
- Métricas normalizadas
- Composición de ingresos (apilado)

**Insight clave**: No hay correlación clara entre precio y satisfacción

---

### 7️⃣ Sección 7: Análisis del Desempeño Geográfico

**Objetivo**: Explorar patrones geográficos de ventas usando coordenadas lat/lon

**Métodos utilizados**:
- `pandas.groupby()` - Agrupación por coordenadas
- `plt.scatter()` - Mapas de dispersión
- `plt.hist2d()` - Mapas de calor (heatmaps)
- Análisis por ciudad
- Anotaciones en gráficos

**Output**:
- Estadísticas de coordenadas únicas por tienda
- Tablas agrupadas por ubicación (Top 10)
- 4 mapas de dispersión (tamaño = ventas, color = ingresos)
- 4 heatmaps de concentración
- Análisis Top 5 ciudades por tienda (doble eje Y)
- Mapa consolidado de 4 tiendas
- Conclusiones geográficas

**Insight clave**: Cada tienda tiene fortalezas regionales específicas

---

### 8️⃣ Informe Final

**Objetivo**: Sintetizar todos los hallazgos y proporcionar recomendación ejecutiva

**Componentes**:
1. **Introducción**: Propósito y metodología
2. **Desarrollo**: Análisis de 7 retos con hallazgos
3. **Tabla Resumen Ejecutivo**: Consolidación de métricas
4. **Análisis FODA**: Fortalezas y debilidades de cada tienda
5. **Matriz de Puntuación Ponderada**: Score multidimensional
   - Ingresos: 30%
   - Calificación: 25%
   - Eficiencia envío: 20%
   - Diversificación: 15%
   - Cobertura geográfica: 10%
6. **Criterios de Decisión**: Escenarios A y B
7. **Recomendación Final**: **VENDER TIENDA 3**
8. **Plan de Acción**: Fases de implementación
9. **Visualización Final**: 4 gráficos consolidados
   - Score ponderado comparativo
   - Matriz Ingresos vs Satisfacción
   - Radar chart multidimensional
   - Contribución al portafolio (pie chart)

**Decisión Final**: 🎯 **Vender Tienda 3** (menor score, menor impacto en portafolio)

---

## 📂 Estructura del Notebook

```
AluraStoreLatam_F.ipynb
│
├── [Celda 1] Importación de datos
│   ├── Carga de 4 datasets desde GitHub
│   └── Exploración inicial (head, info)
│
├── [Sección 1] Análisis de Facturación (2 celdas)
│   ├── Cálculo de ingresos
│   └── Visualización
│
├── [Sección 2] Ventas por Categoría (2 celdas)
│   ├── Value_counts por categoría
│   └── Grid 2x2 de gráficos
│
├── [Sección 3] Calificación Promedio (2 celdas)
│   ├── Mean de calificaciones
│   └── Gráfico con línea de referencia
│
├── [Sección 4] Productos (2 celdas)
│   ├── Ranking de productos
│   └── Top 10 en 4 paneles
│
├── [Sección 5] Envío Promedio (4 celdas)
│   ├── Costo promedio
│   ├── Visualización
│   ├── Tabla resumen consolidada
│   └── Dashboard 4-panel
│
├── [Sección 6] Gráficos Avanzados (6 celdas)
│   ├── Scatter plot
│   ├── Pie chart
│   ├── Boxplot
│   ├── Histogram
│   ├── Line chart
│   └── Stacked bar
│
├── [Sección 7] Análisis Geográfico (8 celdas)
│   ├── Exploración coordenadas
│   ├── Agrupación por ubicación
│   ├── Mapas de dispersión (4)
│   ├── Heatmaps (4)
│   ├── Análisis por ciudad
│   ├── Top 5 ciudades con doble eje
│   ├── Mapa consolidado
│   └── Conclusiones
│
└── [Informe Final] (5 celdas)
    ├── Introducción (markdown)
    ├── Desarrollo del análisis (markdown)
    ├── Tabla resumen ejecutivo (python)
    ├── FODA comparativo (python)
    ├── Scoring ponderado (python)
    ├── Criterios de decisión (markdown)
    ├── Conclusión y recomendación (markdown)
    └── Visualización final (python)
```

**Total**: ~35-40 celdas ejecutables

---

## 📊 Resultados Principales

### Métricas Consolidadas

| Tienda | Ingresos Totales | Calificación | Envío Promedio | Transacciones | Score Total |
|--------|------------------|--------------|----------------|---------------|-------------|
| **Tienda 1** | 🥇 Mayor | 2.99/5 | $17.70 | 2,359 | **100.00** |
| **Tienda 2** | Alto | 3.04/5 | 🥇 $17.59 | 2,074 | 87.50 |
| **Tienda 3** | 🔴 Menor | 2.91/5 | $17.66 | 2,081 | **65.20** |
| **Tienda 4** | Medio | 2.97/5 | $18.16 | 2,085 | 75.80 |

### Decisión Recomendada

> **🎯 VENDER TIENDA 3**

**Razones fundamentadas**:
1. ✅ Menor score ponderado (65.20/100)
2. ✅ Menores ingresos totales del portafolio
3. ✅ Libera capital para reinversión en tiendas rentables
4. ✅ Minimiza riesgo de pérdidas futuras
5. ✅ Menor impacto en ingresos totales (menor pérdida)

**Alternativa**: Si requiere liquidez máxima, vender **Tienda 1** con premium (mayor valoración)

---

## 🗂️ Estructura de Datos

### Datasets Utilizados

Los datos se cargan automáticamente desde GitHub:

```python
url_base = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/main/base-de-datos-challenge1-latam/"

Datasets:
├── tienda_1 .csv  (2,359 transacciones)
├── tienda_2.csv   (2,074 transacciones)
├── tienda_3.csv   (2,081 transacciones)
└── tienda_4.csv   (2,085 transacciones)
```

### Estructura de Columnas

| Nombre de Columna | Tipo | Descripción | Ejemplo |
|-------------------|------|-------------|---------|
| `Producto` | string | Nombre del producto vendido | "Asistente virtual" |
| `Categoría del Producto` | string | Categoría del producto | "Electrónicos" |
| `Precio` | float | Precio de venta (sin envío) | 164300.0 |
| `Costo de envío` | float | Costo del envío | 6900.0 |
| `Fecha de Compra` | string | Fecha de la transacción | "16/01/2021" |
| `Vendedor` | string | Nombre del vendedor | "Pedro Gomez" |
| `Lugar de Compra` | string | Ciudad de compra | "Bogotá" |
| `Calificación` | int | Rating del cliente (1-5) | 4 |
| `Método de pago` | string | Forma de pago | "Tarjeta de crédito" |
| `Cantidad de cuotas` | int | Número de cuotas | 8 |
| `lat` | float | Latitud (coordenada geográfica) | 4.60971 |
| `lon` | float | Longitud (coordenada geográfica) | -74.08175 |

**Total de columnas**: 12  
**Total de registros**: 8,599 transacciones

---

## 🎨 Visualizaciones Incluidas

El notebook genera **25+ visualizaciones profesionales**:

### Gráficos por Reto

| Reto | Tipo de Gráfico | Cantidad |
|------|-----------------|----------|
| Reto 1 | Bar Chart | 1 |
| Reto 2 | Horizontal Bar (4-panel) | 1 |
| Reto 3 | Bar Chart con línea referencia | 1 |
| Reto 4 | Horizontal Bar (4-panel) | 1 |
| Reto 5 | Bar Chart + Dashboard 4-panel | 2 |
| Reto 6 | Scatter, Pie, Box, Hist, Line, Stacked | 6 |
| Reto 7 | Scatter maps (4), Heatmaps (4), Top 5 (4), Consolidado | 13 |
| Informe | Score, Matriz, Radar, Pie | 4 |

**Total**: ~29 visualizaciones

### Características de las Visualizaciones

- ✅ Títulos descriptivos y profesionales
- ✅ Etiquetas en ejes (X, Y)
- ✅ Leyendas cuando aplica
- ✅ Grid para facilitar lectura
- ✅ Colores diferenciados por tienda
- ✅ Anotaciones en puntos clave
- ✅ Tamaños de figura optimizados
- ✅ Formato `tight_layout()` para evitar sobreposiciones
 
 
---

## 📖 Guía de Lectura del Código

### Para principiantes

1. **Empieza por la Sección 1**: Es el más simple y establece las bases
2. **Lee los comentarios**: Cada celda tiene comentarios explicativos
3. **Ejecuta celda por celda**: No ejecutes todo de golpe
4. **Observa los outputs**: Cada celda muestra resultados intermedios

### Para desarrolladores experimentados

- Uso consistente de nombres de variables descriptivos
- Funciones helper para normalización
- Modularidad en visualizaciones (subplots)
- Documentación inline exhaustiva

--- 
### Mejoras sugeridas

- [ ] Agregar análisis de tendencias temporales (por fecha)
- [ ] Implementar modelos predictivos de ventas
- [ ] Crear dashboard interactivo con Plotly
- [ ] Exportar visualizaciones a PDF automáticamente
- [ ] Análisis de vendedores por desempeño
- [ ] Segmentación de clientes por comportamiento
 

    
## Aprendizajes Clave

Al completar este proyecto, habrás aprendido:

✅ Análisis exploratorio de datos (EDA) con pandas  
✅ Visualización de datos con matplotlib  
✅ Manipulación de DataFrames (groupby, agg, value_counts)  
✅ Creación de dashboards con subplots  
✅ Análisis geográfico con coordenadas lat/lon  
✅ Normalización de métricas para comparación  
✅ Elaboración de informes ejecutivos basados en datos  
✅ Toma de decisiones estratégicas con análisis cuantitativo  

 