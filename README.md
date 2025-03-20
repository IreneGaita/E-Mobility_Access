# E-Mobility_Access
## **Analysis of EV Charging Stations Distribution in Italy**

### **Introduction**
The growing adoption of electric vehicles (EVs) necessitates a well-distributed and efficient charging infrastructure. This project analyzes the **geographic distribution of EV charging stations** in Italy, identifies **underserved urban areas**, and develops a **priority map** for new installations. The analysis incorporates factors such as population density, traffic data, and the number of electric vehicles in circulation.

---

### **Objectives**
- **Identify uncovered urban areas**: Determine regions lacking access to a charging station within a reasonable driving range.
- **Define intervention priorities**: Create a priority map to optimize new charging station installations.
- **Map the existing charging network**: Analyze the spatial distribution of charging stations across Italy.
- **Evaluate potential demand**: Compare charging station coverage with population density, traffic, and the number of registered electric vehicles.

---

### **Methodology and Analyses**

#### **1️⃣ Mapping Charging Station Density**
- A **thematic map** was created to visualize charging station density per region.
- Normalization of charging station numbers based on regional surface area.
- Key findings:
  - **Regions with the highest number of stations**: Lombardy (515), Veneto (470), Friuli Venezia Giulia (195).
  - **Regions with the lowest number of stations**: Sardinia (27), Basilicata (9).

#### **2️⃣ Spatial Clustering of Charging Stations**
- Spatial clustering was applied to identify areas with a **high density of charging stations**.
- **Minimum cluster distance**: 2 km
- **Maximum distance between grouped points**: 5 km

#### **3️⃣ Correlation Between Charging Stations and EVs**
- **Pearson Correlation Coefficient = 0.71**, **P-value = 0.0005**.
- A **strong positive correlation** was found between the number of charging stations and the number of electric vehicles in each region.
- Conclusion: **A well-developed charging infrastructure is associated with higher EV adoption.**

#### **4️⃣ Charging Station Saturation Analysis**
- Evaluated whether the existing charging network meets EV demand.
- **High saturation** → Possible congestion, need for additional stations.
- **Low saturation** → More balanced distribution concerning the EV fleet.
- Example results:
  - **Trentino-Alto Adige**: 35,746 EVs, **151 charging stations** (high saturation).
  - **Friuli Venezia Giulia**: 3,632 EVs, **195 charging stations** (low saturation).

#### **5️⃣ Land Use Analysis Using Raster Data**
- By intersecting the **charging station layer** with **CORINE Land Cover (CLC) data**, each station was classified based on land use type.
- Key insights:
  - **72.8% of stations are in urban areas**, with limited presence in rural or agricultural zones.
  - Some stations are located in **non-urban areas**, indicating a growing expansion into less densely populated regions.

#### **6️⃣ Heatmap of Charging Stations Near Strategic Locations**
- A heatmap was created to highlight station concentration near strategic points of interest.
- Key observations:
  - **Highest concentration in continuous urban areas**, aligning with demand.
  - **Significant presence in ports**, likely supporting commercial and tourist traffic.
  - **Coverage along major roads and railways**, supporting long-distance EV travel.

#### **7️⃣ Priority Mapping for New Installations**
- A composite **priority map** was developed by integrating:
  - **EV fleet per region**.
  - **Number of charging stations**.
  - **Population density** (ISTAT data).
- **Z-score normalization** was applied to standardize the values and rank priority areas.

---

### **Technologies and Tools Used**
✅ **QGIS** – GIS analysis and map generation.  
✅ **Python** – Data analysis, clustering, correlation studies.  
✅ **OpenRouteService API** – Used for **isochrone analysis** to measure real-world driving accessibility.  
✅ **Copernicus CORINE Land Cover** – Land use dataset for spatial analysis.  
✅ **ISTAT Data** – Population density dataset for demographic analysis.  

---

## **Key Results and Conclusions**
- **Charging stations are heavily concentrated in urban centers**, with limited expansion into rural areas.
- **The current network shows signs of saturation in certain regions**, highlighting the need for further expansion.
- **Accessibility varies significantly**: Isochrone analysis revealed gaps in charging station coverage, identifying areas where new installations would be most beneficial.
- **The priority map** provides a data-driven approach to optimize future infrastructure investments and accelerate EV adoption in Italy.

---

## Data
Due to GitHub storage limits, large files are stored externally.  
You can download the necessary files from the following link:  

- [Download Material (Google Drive)] (https://drive.google.com/drive/folders/1GoQsoRoxkE2Ndxjz37YJuGbVZpL2zCug?usp=sharing)

After downloading, place the files in the appropriate directory before running the code.

---
#### Author & Contact
📧   **Email**: igaita3107@gmail.com
🔗   **LinkedIn**: www.linkedin.com/in/irene-gaita-4ba32822b


📧  **Email**: m.cicalese21@studenti.unisa.it
🔗  **LinkedIn**: www.linkedin.com/in/mario-cicalese-5b26a5283
