# Coastal Flood Modelling & Risk Assessment: Quelimane, Mozambique

An advanced hydrodynamic flood-modelling project using the open-source **openLISEM** physics engine and **QGIS** to investigate coastal and precipitation-driven flooding in Quelimane, Mozambique. The project focuses on maximum water-level analysis for return-period rainfall scenarios and the assessment of a structural flood-mitigation measure using a 4.0 m dike.

---

## 📍 Study Area

The study area is located in **Quelimane, Mozambique**, a low-lying coastal environment exposed to both precipitation-driven and coastal flooding processes.

---

## 🗄️ Data Source & Availability

The input data (DEM, soil, rainfall and boundary-condition maps, and the location shapefiles for the dike, stadium and test cell) and the base openLISEM script were provided by the UNESCO Open Learning course **"Flood Hazard and Exposure Mapping"** (Hydro-Resilience, 2025), taught by Dr.-Ing. Sardar Ateeq and Steven Huysentruyt (Antea Group Belgium). This project was completed as the final project of that course.

The raster files (`.map`, `.tif`, `.tiff`) — both the course input data and the simulated maximum water-level outputs — and the course shapefiles in `02_Original_Data/Locations/` are **not included in this repository**: the rasters are too large, and the course data are not redistributed here. To reproduce the simulations, obtain the input data from the course and place them in `02_Original_Data/` following the folder structure below.

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
Quelimane_Flood_Project/
│
├── README.md
├── .gitignore
│
├── 02_Original_Data/
│   ├── Log_files/          # CSV time-series outputs of the simulations
│   ├── Input/              # not on GitHub – see Data Source & Availability
│   ├── Locations/          # not on GitHub – see Data Source & Availability
│   ├── Rain/               # not on GitHub – see Data Source & Availability
│   └── Results/            # not on GitHub – see Data Source & Availability
│
├── 03_Simulations/
│   └── Scripts/            # openLISEM scenario scripts
│
├── 04_QGIS_Project/
│   ├── Flood_Modelling_Quelimane.qgz
│   ├── Hydrograph/
│   ├── Layout/
│   └── Symbology/
│
└── 05_Reports/
    └── Final_Maps/
        ├── Flood_Risk_Mitigation_Comparison/
        └── Maximum_Water_Level_Comparison_T50_10_Hours/
```

### `02_Original_Data/`

- `Log_files/` – CSV time-series outputs generated from the flood simulations, including rainfall, no-rainfall, and dike-scenario monitoring results.
- `Input/` – DEM, soil and hydraulic parameter maps, and boundary-condition rasters used by the model *(local only)*.
- `Locations/` – Shapefiles of the dike, stadium, and test-cell location *(local only)*.
- `Rain/` – Rainfall input maps for the T10, T20, and T50 return-period scenarios *(local only)*.
- `Results/` – Spatially distributed maximum water-level simulation outputs *(local only)*.

The folders marked *local only* are kept on the author's computer and are excluded from GitHub through `.gitignore`; see **Data Source & Availability** above.

### `03_Simulations/`

- `Scripts/` – openLISEM scripts: the base T50 script (`Code.script`), the T50 stadium analysis with and without rainfall, and the 5-day 4.7 m scenarios with and without the 4.0 m dike.

### `04_QGIS_Project/`

Contains the QGIS project and GIS analysis/presentation materials:

- `Flood_Modelling_Quelimane.qgz` – Master QGIS project.
- `Hydrograph/` – Generated analysis figures and hydrograph-related visualisations.
- `Layout/` – Saved QGIS print-layout templates (`.qpt`) for the project maps.
- `Symbology/` – Saved QGIS layer styles (`.qml`) used for consistent map presentation.

### `05_Reports/`

- `Final_Maps/` – Final presentation-ready maps (PNG and PDF).

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
- **Extreme sea level:** 4.7 m
- **Rainfall:** No rainfall
- **Monitoring cell:** Column `1014`, Row `1042`

The mitigation scenario is compared with the corresponding condition without the dike to assess changes in maximum water level.

---

## 🌧️ T50 Maximum Water Level Comparison

A separate comparison analysis was produced for the **T50 maximum water level** under:

- **10-hour simulation** (rainfall applied during the first 6 hours)
- **6.5 m extreme sea level**
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
- Extreme-sea-level scenario analysis
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
