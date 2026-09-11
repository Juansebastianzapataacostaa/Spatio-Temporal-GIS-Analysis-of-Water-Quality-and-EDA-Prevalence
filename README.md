# Spatio-Temporal GIS Analysis of Water Quality and EDA Prevalence in Colombia

## Project Overview
This geospatial analytics project leverages **ArcGIS Pro** to evaluate the spatio-temporal evolution of water quality across Colombia's departments. It operationalizes the Water Quality Risk Index (**IRCA**) and contrasts it against the prevalence of Acute Diarrheal Diseases (**EDA**) using national epidemiological surveillance registries (**SIVICAP** and **SIVIGILA**).

The objective is to establish an automated, scalable data-engineering and cartographic workflow to monitor environmental public health indicators, assess administrative reporting compliance, and validate spatial correlations between water security and population vulnerability.

---

## Repository Data Architecture (`data/` Directory)

To ensure full transparency and data reproducibility, the processed and structured data streams are organized as follows:

- 📄 `colombia_incidencias_eda_2014_2020.csv`: Consolidated public health matrix containing the total number of notified cases and computed incidence rates per 1,000 inhabitants for Acute Diarrheal Diseases (EDA) across all departments. Includes demographic baselines derived from DANE censuses.
- 📄 `irca_promedios_anuales_2014_2018.csv`: Annualized environmental baseline matrix that summarizes the average IRCA values for Colombia's 32 departments and Bogotá D.C. used for the primary thematic map rendering.
- 📄 `irca_series_temporales_2015_2018.csv`: Intermediate time-series data table documenting cross-year calculated risk means used to evaluate directional variations in water safety.
- 📦 `gadm36_COL_shp.zip`: Geodatabase compressed archive containing the official GADM vector shapefiles (polygons and spatial boundaries) at the departmental level for Colombia.

---

## Key Methodological Workflows

### 1. Data Cleaning & Geodatabase Integration
- Filtered and structured extensive national health registries, isolating missing parameters and external geographic noise.
- Engineered a structured **File Geodatabase (GDB)** inside ArcGIS Pro integrated with the **GADM** administrative area layers.

### 2. Spatial Analysis & Cartography
- Executed image georeferencing workflows and control point assignment via 1st-order polynomial (Affine) transformations.
- Digitized shapefiles, managed coordinate reference systems, and generated multi-layer choropleth maps using automated color-indexing scales.

### 3. Statistical Modeling & QA/QC
- Programmed multi-variable linear regressions and computed $R^2$ trendlines to evaluate dependency mechanics between IRCA risk spikes and regional morbidity/mortality outputs.
- Applied rigorous Quality Assurance / Quality Control (QA/QC) topologies to enforce data consistency across boundary intersections.

---

## Core Technical Stack
- **GIS Software:** ArcGIS Pro, Geodatabase (GDB) Architecture, ArcGIS Online.
- **Languages & Frameworks:** Python (ArcPy syntax ready), SQL queries, Markdown.
- **Analytics Tools:** Microsoft Excel, Data Table Optimization, Attribute Mapping, Topological Validation.

---

## Main Deliverable
- `GIS_Spatial_Analysis_Portfolio_Juan_Zapata.pdf`: Complete, executive research manuscript containing methodology, multi-layer layout maps, correlation plots, and geospatial validation discussion.

---
*Developed as an independent geospatial research pipeline by Juan Sebastian Zapata Acosta.*
