# Olist Customer Analytics

Proyecto de **Customer Analytics** basado en el dataset público **Brazilian E-Commerce Public Dataset by Olist**.

El objetivo principal del proyecto es practicar el flujo completo de trabajo analítico, desde la preparación de datos hasta la construcción de un cuadro de mando en **Power BI**, aplicando conceptos como segmentación RFM, churn, retención, cohortes, CLV y priorización de acciones.

---

## Objetivo del proyecto

Este proyecto tiene como finalidad desarrollar un caso práctico de análisis de clientes utilizando datos de ecommerce.

Los objetivos principales son:

* preparar y transformar los datos mediante un proceso ETL;
* analizar la evolución de clientes, pedidos e ingresos;
* construir métricas de volumen de clientes;
* desarrollar una segmentación RFM;
* analizar churn y retención;
* construir cohortes de clientes;
* calcular métricas de valor como AOV, ARPU y CLV;
* simular variables adicionales si son necesarias;
* diseñar recomendaciones y acciones de negocio;
* construir un dashboard interactivo en Power BI.

---

## Dataset

El proyecto utiliza el dataset público **Brazilian E-Commerce Public Dataset by Olist**, disponible en Kaggle.

Los archivos originales del dataset no se incluyen en este repositorio. Deben descargarse manualmente y colocarse en la carpeta:

```text
data/raw/
```

Archivos esperados:

```text
olist_customers_dataset.csv
olist_geolocation_dataset.csv
olist_order_items_dataset.csv
olist_order_payments_dataset.csv
olist_order_reviews_dataset.csv
olist_orders_dataset.csv
olist_products_dataset.csv
olist_sellers_dataset.csv
product_category_name_translation.csv
```

---

## Estructura del repositorio

```text
olist-customer-analytics/
│
├── assets/
├── dashboards/
├── data/
│   ├── raw/
│   ├── clean/
│   ├── processed/
│   └── simulated/
├── docs/
├── notebooks/
├── reports/
├── scripts/
├── sql/
├── .gitignore
├── README.md
└── requirements.txt
```

---

## Descripción de carpetas

| Carpeta           | Descripción                                                      |
| ----------------- | ---------------------------------------------------------------- |
| `data/raw/`       | Datos originales descargados de Kaggle. No se versionan en Git.  |
| `data/clean/`     | Datos limpiados o transformaciones intermedias.                  |
| `data/processed/` | Tablas finales preparadas para Power BI.                         |
| `data/simulated/` | Variables o tablas simuladas para enriquecer el análisis.        |
| `notebooks/`      | Notebooks de exploración, limpieza, transformación y simulación. |
| `scripts/`        | Scripts reutilizables de Python.                                 |
| `sql/`            | Consultas SQL, si se utilizan durante el proyecto.               |
| `dashboards/`     | Archivos del dashboard de Power BI.                              |
| `docs/`           | Documentación metodológica del proyecto.                         |
| `reports/`        | Capturas, informes o entregables derivados del análisis.         |
| `assets/`         | Imágenes, iconos u otros recursos visuales.                      |

---

## Principales áreas de análisis

El proyecto se organizará en torno a las siguientes áreas:

1. **Volumen de clientes**

   * clientes totales;
   * clientes activos;
   * clientes nuevos;
   * clientes perdidos;
   * crecimiento neto.

2. **Segmentación RFM**

   * recency;
   * frequency;
   * monetary;
   * clasificación de clientes;
   * segmentos accionables.

3. **Churn y retención**

   * definición de cliente perdido;
   * churn rate;
   * retention rate;
   * clientes en riesgo;
   * motivo de baja, si está disponible o puede simularse.

4. **Cohortes**

   * cohortes por primera compra;
   * evolución de la retención;
   * comparación entre cohortes con la misma madurez.

5. **Valor del cliente**

   * revenue;
   * AOV;
   * ARPU;
   * CLV histórico o aproximado;
   * clientes de alto valor.

6. **Acciones y recomendaciones**

   * priorización de clientes;
   * reglas de negocio;
   * acciones recomendadas;
   * simulación de seguimiento operativo si es necesario.

7. **Dashboard en Power BI**

   * modelo relacional;
   * medidas DAX;
   * visualizaciones interactivas;
   * navegación entre páginas;
   * storytelling ejecutivo.

---

## Flujo de trabajo previsto

```text
Datos originales
→ Exploración inicial
→ Validación de calidad
→ Limpieza y transformación
→ Simulación de variables, si procede
→ Preparación de tablas finales
→ Modelado en Power BI
→ Creación de medidas DAX
→ Construcción del dashboard
→ Documentación de decisiones metodológicas
```

---

## Herramientas utilizadas

* Python
* Pandas
* NumPy
* Jupyter Notebooks
* Power BI
* DAX
* Git / GitHub
* GitHub Desktop

---

## Nota metodológica

Los datos originales proceden del dataset público de Olist. Cualquier variable adicional que no exista en la fuente original, como acciones recomendadas, estado de tareas, prioridad comercial o determinadas clasificaciones de riesgo, será simulada de forma controlada y documentada.

El objetivo no es únicamente construir un dashboard visual, sino practicar un flujo de trabajo analítico completo y justificar las decisiones tomadas durante el proceso.
