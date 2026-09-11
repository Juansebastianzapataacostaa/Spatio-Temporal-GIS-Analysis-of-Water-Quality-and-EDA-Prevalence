# Spatio-Temporal GIS Analysis of Water Quality and EDA Prevalence in Colombia

## Project Overview
This geospatial analytics project leverages **ArcGIS Pro** to evaluate the spatio-temporal evolution of water quality across Colombia's departments, operationalizing the Water Quality Risk Index (**IRCA**) and contrasting it against the prevalence of Acute Diarrheal Diseases (**EDA**) using national surveillance registries (**SIVICAP** and **SIVIGILA**).

The objective is to establish an automated, scalable data-engineering and cartographic workflow to monitor environmental public health indicators, assess administrative reporting compliance, and validate spatial correlations between water security and population vulnerability.

---

## Key Methodological Workflows

### 1. Data Cleaning & Geodatabase Integration
- Managed, filtered, and cleaned extensive national health registries, isolating missing parameters and external geographic noise.
- Engineered a structured **File Geodatabase (GDB)** inside ArcGIS Pro integrated with the **GADM** global administrative areas boundaries layer at the departmental level for Colombia.

### 2. Spatial Analysis & Cartography
- Executed image georeferencing workflows and control point assignment via 1st-order polynomial (Affine) transformations.
- Digitized shapefiles, managed diverse coordinate reference systems, and generated multi-layer choropleth maps using automated color-indexing scales.
- Tracked demographic variables and epidemiological incidence targets computed per 100,000 inhabitants.

### 3. Statistical Modeling & QA/QC
- Programmed multi-variable linear regressions and computed $R^2$ trendlines to evaluate dependency mechanics between IRCA risk spikes and regional morbidity/mortality outputs.
- Applied rigorous Quality Assurance / Quality Control (QA/QC) topologies to enforce data consistency and topological rule validation across boundary intersections.

---

## Core Technical Stack
- **GIS Software:** ArcGIS Pro, Geodatabase (GDB) Architecture, ArcGIS Online.
- **Data Layers:** GADM Global Administrative Vector Polygons, SIVICAP, SIVIGILA.
- **Analytics & Documentation:** Data Table Optimization, Attribute Mapping, Topological Validation.

---

## Project Repository Structure
- `GIS_Spatial_Analysis_Portfolio_Juan_Zapata.pdf`: Complete, executive peer-reviewed research manuscript containing methodology, multi-layer maps, correlation plots, and geospatial validation discussion.

---
*Developed as an independent geospatial research pipeline by Juan Sebastian Zapata Acosta.*
