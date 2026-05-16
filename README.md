 # 🌍 Land Surface Temperature Analysis of Offa LGA (2014–2024)

![GIS](https://img.shields.io/badge/Field-GIS-blue)
![Remote Sensing](https://img.shields.io/badge/Skill-Remote%20Sensing-green)
![ArcGIS Pro](https://img.shields.io/badge/Tool-ArcGIS%20Pro-orange)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)
![Focus](https://img.shields.io/badge/Focus-Urban%20Climate%20Analysis-red)

---

##  Table of Contents
- [Project Overview](#project-overview)
- [ Objectives](#objectives)
- [ Study Area](#study-area)
- [ Data Sources](#data-sources)
- [ Tools & Technologies](#tools--technologies)
- [ Methodology](#methodology)
- [ Results & Insights](#results--insights)
- [ Spatial Analysis](#spatial-analysis)
- [ Interpretation](#interpretation)
- [ Conclusion](#conclusion)
- [ Recommendations](#recommendations)
 

---

## Project Overview

Urban expansion is significantly altering local climate systems. This project analyzes **Land Surface Temperature (LST)** changes in Offa LGA over a 10-year period using satellite imagery.

By integrating **Remote Sensing and GIS**, this study identifies temperature patterns, vegetation loss, and the emergence of **Urban Heat Island (UHI)** effects.

---

##  Objectives

- Analyze **LST variation (2014 vs 2024)**
- Identify **Urban Heat Island patterns**
- Evaluate impact of **urbanization on temperature**
- Support **climate resilience and planning decisions**

---

##  Study Area

📍 Offa Local Government Area, Kwara State, Nigeria  

- Predominantly agricultural region  
- Experiencing gradual urban expansion  
- Suitable for environmental change detection  
<img width="4134" height="5846" alt="OFFA" src="https://github.com/user-attachments/assets/0e5c6fe7-335c-4a4d-bb89-da66a80fcce8" />

---

##  Data Sources

| Data | Source | Purpose |
|------|--------|--------|
| Landsat 8 Imagery | USGS Earth Explorer | LST Analysis |
| Band 10 & 11 | Thermal Bands | Temperature Extraction |
| Band 4 & 5 | Red & NIR | NDVI Calculation |

**Years Analyzed:** 2014 & 2024  

---

##  Tools & Technologies

- ArcGIS Pro  
- Remote Sensing Techniques  
- Raster Analysis  
- Microsoft Excel  

---

##  Methodology

### 1. Data Preprocessing
- Import Landsat imagery into ArcGIS Pro  
- Extract thermal bands  
- Apply **Cell Statistics (Mean)**  

---


 ## 🔄 Methodology (Detailed Computation Workflow)

---

### 2. Radiometric Conversion (DN → TOA Radiance)

Lλ = ML × Qcal + AL

**Aim:**  
To convert raw satellite data into physically meaningful radiance values.

**Objective:**  
To transform Digital Number (DN) values into Top of Atmosphere (TOA) spectral radiance using calibration parameters for accurate thermal analysis.

---

### 3. Brightness Temperature (Radiance → Temperature)

BT = K2 / ln((K1 / Lλ) + 1)

BT (°C) = BT (K) − 273.15

**Aim:**  
To estimate the surface temperature as detected by the satellite sensor.

**Objective:**  
To convert spectral radiance into brightness temperature using thermal constants, and express the result in Celsius for interpretation.

---

### 4. NDVI Calculation (Vegetation Detection)

NDVI = (NIR − Red) / (NIR + Red)

**Aim:**  
To assess vegetation presence and density within the study area.

**Objective:**  
To compute vegetation index values using red and near-infrared bands for distinguishing vegetated and non-vegetated surfaces.

---

### 5. Proportion of Vegetation (Pv)

Pv = ((NDVI − NDVImin) / (NDVImax − NDVImin))²

**Aim:**  
To quantify the extent of vegetation cover across the study area.

**Objective:**  
To normalize NDVI values and derive the fractional vegetation cover required for emissivity estimation.

---

### 6. Land Surface Emissivity (LSE)

ε = 0.004Pv + 0.986

**Aim:**  
To account for variations in surface material properties affecting heat emission.

**Objective:**  
To estimate surface emissivity based on vegetation proportion, improving the accuracy of temperature calculations.

---

### 7. Land Surface Temperature (LST)

LST = BT / (1 + (λ × BT / c₂) × ln(ε))

**Aim:**  
To derive the actual land surface temperature of the study area.

**Objective:**  
To integrate brightness temperature and emissivity corrections to compute accurate LST values for environmental analysis.
---



 

##  Results & Insights

| Year | Min Temp | Max Temp |
|------|---------|---------|
| 2014 | 23.15°C | 31.41°C |
| 2024 | 26.16°C | 35.66°C |

### 🔍 Key Findings

- 🔺 Temperature increased by **~4°C**
- 🔴 Expansion of **urban heat zones**
- 🟢 Decline in **vegetation cover**
- 🌆 Strong **Urban Heat Island effect**


 <img width="5846" height="4134" alt="LST" src="https://github.com/user-attachments/assets/4fd1a64f-874e-4513-a0a5-1f273137dd6f" />

---

##  Spatial Analysis

- 🟢 **Cool Areas:** Vegetation & water bodies  
- 🟡 **Moderate:** Mixed land use  
- 🔴 **Hot Areas:** Built-up & bare land  

📌 2024 shows increased **heat concentration and urban spread**

---

##  Interpretation

The observed temperature rise is driven by:

- Urban expansion  
- Vegetation loss  
- Increase in impervious surfaces  

➡️ Clear evidence of **human-induced climate impact**

---

##  Conclusion

This study reveals a **significant increase in Land Surface Temperature** over a decade.

It demonstrates how GIS and Remote Sensing can:

- Monitor environmental changes  
- Support urban planning  
- Enable climate adaptation strategies  

---

##  Recommendations

- 🌱 Promote urban greening  
- 🏗️ Adopt climate-smart infrastructure  
- 🛰️ Implement continuous satellite monitoring  

 

 

 

 

