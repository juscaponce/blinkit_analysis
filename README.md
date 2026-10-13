<img width="1256" height="621" alt="image" src="https://github.com/user-attachments/assets/08af1a8f-746e-40aa-87a2-7be918021f51" /># 📊 Análisis de Desempeño de Ventas, Satisfacción del Cliente e Inventario — Blinkit (Power BI)
## 📌 Descripción del Proyecto
Este proyecto consiste en el desarrollo de una solución analítica e interactiva en **Microsoft Power BI** para **Blinkit**. Su objetivo principal es evaluar el desempeño de las ventas, comprender los patrones de satisfacción de los clientes y optimizar la distribución del inventario en los diferentes tipos de establecimientos (*outlets*).

Mediante el uso de indicadores clave de desempeño (KPIs) y visualizaciones dinámicas, el dashboard permite identificar oportunidades de optimización operativa y comercial.
VISTA PREVIA
---

## 🎯 Objetivos de Negocio
* **Desempeño Comercial:** Analizar los impulsores de ingresos a través de los atributos de los productos (contenido de grasa, categoría de ítem).
* **Satisfacción del Cliente:** Monitorear la experiencia del usuario evaluando la calificación promedio por tipología de producto y punto de venta.
* **Distribución y Cobertura:** Evaluar la eficiencia operativa según el tamaño, la ubicación geográfica y la antigüedad de los canales de venta.

---

## 🔑 Indicadores Clave de Desempeño (KPIs)

En la sección superior del dashboard se presentan cuatro métricas clave estructuradas mediante tarjetas (*Card Visuals*):

| KPI | Descripción | 
| :--- | :--- |
| **Total Sales** | Ingresos brutos acumulados por la totalidad de productos vendidos. | 
| **Average Sales** | Ingreso promedio generado por transacción o producto comercializado. | 
| **Number of Items** | Conteo total de artículos o SKUs distintos vendidos. | 
| **Average Rating** | Valoración promedio de satisfacción otorgada por los clientes. |

---

## 🔍 Requerimientos Analíticos Granulares

### 1. Total Sales by Fat Content (Ventas Totales por Contenido de Grasa)
* **Objetivo:** Determinar la influencia del contenido de grasa (*Low Fat*, *Regular*) sobre el total de ventas.
* **Métricas Adicionales Evaluadas:** *Average Sales*, *Number of Items* y *Average Rating* segundas por tipo de contenido graso.
* **Visualización:** Gráfico de Donas / Pie Chart y matriz analítica cruzada.

### 2. Total Sales by Item Type (Ventas Totales por Tipo de Producto)
* **Objetivo:** Identificar el rendimiento comercial y participación de mercado de las distintas categorías (*Snacks, Dairy, Frozen Foods, Soft Drinks, etc.*).
* **Métricas Adicionales Evaluadas:** Variación de *Average Sales*, *Number of Items* y *Average Rating* según la categoría del producto.
* **Visualización:** Gráfico de Barras Horizontales ordenado descendentemente.

### 3. Fat Content by Outlet for Total Sales (Contenido de Grasa por Outlet)
* **Objetivo:** Comparar la distribución de ventas por contenido de grasa desglosado entre los diferentes puntos de venta (*Outlets*).
* **Métricas Adicionales Evaluadas:** Comportamiento de *Average Sales*, *Number of Items* y *Average Rating* por combinación de Outlet y Fat Content.
* **Visualización:** Gráfico de Barras Apiladas (*Stacked Bar Chart*).

### 4. Total Sales by Outlet Establishment (Ventas Totales por Año de Establecimiento)
* **Objetivo:** Evaluar cómo la antigüedad o año de fundación (*Establishment Year*) del outlet influye en el volumen de ventas generado.
* **Visualización:** Gráfico de Líneas de Tendencia Temporal / Columnas Clustered por Año.

---

## 📈 Requerimientos de Visualizaciones y Gráficos

### 5. Percentage of Sales by Outlet Size (Porcentaje de Ventas por Tamaño de Outlet)
* **Objetivo:** Analizar la correlación entre el tamaño de la tienda (*Small, Medium, High/Large*) y su contribución porcentual al total de ventas.
* **Visualización:** Donut Chart (% de participación del total de ventas).

### 6. Sales by Outlet Location (Ventas por Ubicación del Outlet)
* **Objetivo:** Mapear la distribución geográfica e ingresos según el nivel/zona de ubicación (*Tier 1, Tier 2, Tier 3*).
* **Visualización:** Gráfico de Embudo (*Funnel Chart*) o Mapa Coroplético.

### 7. All Metrics by Outlet Type (Consolidado de Métricas por Tipo de Outlet)
* **Objetivo:** Proporcionar una vista integral y ejecutiva que reúna todas las métricas clave (*Total Sales, Average Sales, Number of Items, Average Rating*) desglosadas por tipo de canal (*Supermarket Type1, Type2, Type3, Grocery Store*).
* **Visualización:** Tabla Matricial (*Matrix Visual*) con barras de datos condicionales.


## 📁 Estructura del Repositorio

```text
├── data/
│   └── blinkIT Grocery Data       # Dataset original
├── docs/
│   └── BRD_Blinkit_PowerBI.docx   # Documento de Requerimientos de Negocio
├── powerbi/
│   └── Blinkit_Sales_Analysis.pbix # Archivo ejecutable de Power BI
└── README.md                      # Documentación principal
