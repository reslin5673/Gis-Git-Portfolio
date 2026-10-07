# Coastal Flood Modelling & Risk Assessment: Quelimane, Mozambique

An advanced hydrodynamic flood-modelling project using the open-source **openLISEM** physics engine and **QGIS** to investigate coastal and precipitation-driven flooding in Quelimane, Mozambique. The project focuses on maximum water-level analysis for return-period rainfall scenarios and the assessment of a structural flood-mitigation measure using a 4.0 m dike.

---

## 📍 Study Area

The study area is located in **Quelimane, Mozambique**, a low-lying coastal environment exposed to both precipitation-driven and coastal flooding processes.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Simulate flood conditions using **openLISEM**.
- Investigate maximum water levels under different rainfall and sea-level conditions.
- Analyse flood behaviour at selected critical locations.
- Compare maximum water levels under rainfall and no-rainfall conditions.
- Evaluate the effect of a **4.0 m high dike** as a structural flood-mitigation measure.
- Analyse and communicate flood-modelling results using **QGIS**.
- Produce professional comparative flood maps and visualisations.

---

## 📂 Repository Structure

```text
Flood-Modelling-Quelimane/
│
├── 01_Readme.md
│
├── 02_Original_Data/
│   ├── Input/
│   ├── Log_files/
│   ├── Locations/
│   ├── Rain/
│   └── Results/
│
├── 03_Simulations/
│
├── 04_QGIS_Project/
│   ├── Flood_Modelling_Quelimane.qgz
│   ├── Hydrograph/
│   ├── Symbology/
│   └── Layouts/
│
├── 05_Reports/
│   └── Final_Maps/
│
├── 06_Resources/
│
└── 07_Project_Aim/
```

### `02_Original_Data/`

- `Input/` – DEM, soil and hydraulic parameter maps, and boundary-condition rasters used by the model.
- `Log_files/` – CSV time-series outputs generated from the flood simulations, including rainfall, no-rainfall, and dike-scenario monitoring results.
- `Locations/` – Spatial shapefiles including the dike, stadium, and project location markers.
- `Rain/` – Rainfall input maps for the T10, T20, and T50 return-period scenarios.
- `Results/` – Spatially distributed maximum water-level simulation outputs.

### `03_Simulations/`

Contains the openLISEM simulation workflow, model configurations, scenario-specific settings, and simulation-related files.

### `04_QGIS_Project/`

Contains the QGIS project and GIS analysis/presentation materials:

- `Flood_Modelling_Quelimane.qgz` – Master QGIS project.
- `Hydrograph/` – Generated analysis figures and hydrograph-related visualisations.
- `Symbology/` – Saved QGIS layer styles (`.qml`) used for consistent map presentation.
- `Layouts/` – Saved QGIS print-layout templates (`.qpt`) for the project maps.

### `05_Reports/`

Contains final project outputs and presentation-ready maps.

### `06_Resources/`

Contains supporting project resources, assignment material, course references, and background documentation.

### `07_Project_Aim/`

Contains the project aim and related project-definition material.

---

## 🚀 Technical Tasks & Frameworks

### 📍 Task 1: Flood Onset Detection at a Critical Location

The first task evaluates flood behaviour at the **Campo CFM Football Stadium** located at:

- **Grid cell:** Column `1018`, Row `1041`
- **Scenario:** T50 rainfall combined with the relevant coastal boundary conditions.

The analysis focuses on identifying the temporal development of flooding at the selected critical location and investigating the contribution of rainfall and coastal forcing.

### 🛠️ Task 2: Structural Mitigation Scenario Testing

The second task evaluates a structural flood-mitigation scenario using a simulated:

- **Dike height:** 4.0 m
- **Simulation duration:** 5 days
- **Sea-level rise:** 4.7 m
- **Rainfall:** No rainfall
- **Monitoring cell:** Column `1014`, Row `1042`

The mitigation scenario is compared with the corresponding condition without the dike to assess changes in maximum water level.

---

## 🌧️ T50 Maximum Water Level Comparison

A separate comparison analysis was produced for the **T50 maximum water level** under:

- **6-hour simulation**
- **6.5 m sea-level rise**
- **With rainfall**
- **Without rainfall**

The resulting maps compare the spatial distribution of maximum water level between the rainfall and no-rainfall conditions.

---

## ⚙️ Modelling Workflow

```text
Input Data
    ↓
DEM & Model Preparation
    ↓
Rainfall / Sea-Level Boundary Conditions
    ↓
openLISEM Configuration
    ↓
Flood Simulation
    ↓
Time-Series & Maximum Water-Level Analysis
    ↓
QGIS Spatial Analysis
    ↓
Scenario Comparison
    ↓
Flood-Mitigation Assessment
    ↓
Final Maps & Visualisations
```

---

## 📊 Key Visualisations & Results

### Hydrographic Profiling

Time-series and hydrograph-related figures were generated to investigate flood behaviour and maximum water-level differences at selected locations.

### Spatial Flood Comparison

QGIS was used to create comparative maximum-water-level maps for:

1. **T50 rainfall vs. no-rainfall conditions**
2. **Without dike vs. 4.0 m dike mitigation conditions**

The final cartographic layouts include legends, north arrows, scale bars, location markers, and scenario-specific map titles.

---

## 🗺️ Final Maps

The final presentation-ready maps are stored in:

```text
05_Reports/Final_Maps/
```

Current final map outputs include:

- **Flood Risk Mitigation Comparison**
- **T50 Maximum Water Level Comparison**

---

## 🛠️ Technologies & Tools Applied

- **openLISEM** – Physically based distributed hydrological and flood modelling.
- **QGIS Desktop** – Raster and vector GIS analysis, spatial visualisation, symbology, and print-layout design.
- **Microsoft Excel** – Time-series processing, matrix calculations, and data visualisation.
- **Git & GitHub** – Version control and professional project documentation.

---

## 🔑 Skills Demonstrated

- Flood modelling
- Hydrodynamic modelling
- openLISEM
- QGIS
- Raster data processing
- Vector data processing
- DEM analysis
- Flood scenario comparison
- Sea-level-rise scenario analysis
- Flood-mitigation assessment
- GIS cartography
- Time-series analysis
- Technical project organisation
- Git and GitHub

---

## 👤 Author

**Reslin C.R.**

M.Sc. Hydro Environmental Extremes  
University of Siegen, Germany
