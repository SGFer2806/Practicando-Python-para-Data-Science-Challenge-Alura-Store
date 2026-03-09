# 🛒 Alura Store Latam — Análisis de Rendimiento

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7+-orange)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-F9AB00?logo=googlecolab&logoColor=white)

---

## 📌 Propósito del Análisis

El Sr. Juan es dueño de una cadena de 4 tiendas llamada **Alura Store** y desea vender una de ellas para financiar un nuevo emprendimiento. El objetivo de este proyecto es **identificar cuál tienda tiene el peor rendimiento** analizando datos reales de ventas, para entregar una recomendación fundamentada en evidencia.

Las preguntas clave que guían el análisis son:

- ¿Cuál tienda genera menos ingresos?
- ¿Cuál tiene peores calificaciones de clientes?
- ¿Qué tienda vende menos productos?
- ¿Cómo se comparan los costos de envío y precios promedio?

---

## 📁 Estructura del Proyecto

```
AluraStore/
│
├── AluraStoreLatam_Completo.ipynb   # Notebook principal con todo el análisis
├── README.md                        # Este archivo
│
└── datos/                           # Fuentes de datos (cargadas vía URL)
    ├── tienda_1.csv
    ├── tienda_2.csv
    ├── tienda_3.csv
    └── tienda_4.csv
```

> 💡 Los datos se cargan directamente desde el repositorio oficial de Alura en GitHub, por lo que no es necesario descargar los archivos CSV manualmente.

---

## 🔍 Estructura del Notebook

El notebook está organizado en 7 secciones:

| # | Sección | Descripción |
|---|---------|-------------|
| 1 | 📥 Importación de datos | Carga las 4 tiendas con Pandas y las unifica |
| 2 | 💰 Facturación | Ingresos totales (precio + envío) por tienda |
| 3 | 📦 Ventas por categoría | Qué categorías dominan en cada tienda |
| 4 | ⭐ Calificación promedio | Satisfacción del cliente por tienda |
| 5 | 🏆 Productos más/menos vendidos | Top 5 y bottom 5 de cada tienda |
| 6 | 🚚 Envío promedio | Costo de envío y dispersión precio/envío |
| 7 | 📝 Recomendación final | Conclusión argumentada con los datos |

---

## 📊 Gráficos e Insights Obtenidos

### 1. Facturación Total por Tienda
> **Gráfico:** Barras verticales comparando ingresos totales.

**Insight:** La Tienda 1 lidera ampliamente en facturación, mientras que la **Tienda 4 registra los ingresos más bajos** de toda la cadena.

---

### 2. Ventas por Categoría
> **Gráfico:** Barras agrupadas por categoría y tienda.

**Insight:** Todas las tiendas tienen un mix de categorías similar, dominado por *Electrónicos* y *Muebles*. La Tienda 4 muestra volúmenes consistentemente menores en todas las categorías.

---

### 3. Distribución de Calificaciones
> **Gráfico:** 4 gráficos de pastel (uno por tienda) mostrando el % de cada puntuación (1–5 estrellas).

**Insight:** La **Tienda 4 tiene el promedio de calificación más bajo**, con mayor proporción de reseñas de 1 y 2 estrellas respecto a las demás.

---

### 4. Productos Más Vendidos
> **Gráfico:** Barras horizontales con el Top 5 de productos por tienda.

**Insight:** Los productos líderes varían entre tiendas. La Tienda 1 y Tienda 2 tienen productos con volúmenes de venta notablemente superiores.

---

### 5. Precio Promedio vs. Costo de Envío
> **Gráfico:** Dispersión donde el tamaño del punto representa el número de ventas.

**Insight:** La Tienda 4 tiene el menor tamaño de burbuja (menos ventas), además de los valores más bajos de precio y envío promedio, lo que se traduce en márgenes reducidos sin compensación por volumen.

---

### 6. Comparación Normalizada de Indicadores
> **Gráfico:** Líneas multieje con métricas normalizadas (0 = peor, 1 = mejor).

**Insight:** La Tienda 4 aparece consistentemente en los valores más bajos en facturación, volumen y calificación. Es el patrón más claro para la toma de decisión.

---

## ✅ Recomendación Final

> **El Sr. Juan debería vender la Tienda 4.**

Los datos muestran de forma consistente que la Tienda 4 es la menos eficiente en todos los indicadores evaluados: menor facturación, menor número de ventas, peor calificación promedio de clientes y márgenes reducidos. Venderla representa la menor pérdida de valor para la cadena y libera capital para invertir en un nuevo emprendimiento.

---

## ▶️ Instrucciones para Ejecutar el Notebook

### Opción 1 — Google Colab (recomendado)

1. Descarga el archivo `AluraStoreLatam_Completo.ipynb`.
2. Ve a [colab.research.google.com](https://colab.research.google.com).
3. Haz clic en **Archivo → Subir notebook** y selecciona el archivo.
4. Ejecuta todas las celdas con **Runtime → Run all** (o `Ctrl + F9`).

> No se necesita instalar nada. Pandas y Matplotlib ya están disponibles en Colab.

### Opción 2 — Entorno local

Asegúrate de tener Python 3.10+ instalado, luego ejecuta:

```bash
# Instalar dependencias
pip install pandas matplotlib numpy jupyter

# Abrir el notebook
jupyter notebook AluraStoreLatam_Completo.ipynb
```

### Dependencias

| Librería | Versión mínima | Uso |
|----------|---------------|-----|
| `pandas` | 1.5+ | Carga y manipulación de datos |
| `matplotlib` | 3.5+ | Visualización de gráficos |
| `numpy` | 1.23+ | Operaciones numéricas |

---

## 👤 Autor
Fernando Santos García
Proyecto desarrollado como parte del **Challenge 1 de Data Science — Alura Latam**.

---

*Datos proporcionados por [Alura Latam](https://github.com/alura-es-cursos/challenge1-data-science-latam)*