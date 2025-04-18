# Public Health Research Report and Presentation  
## Geospatial Influenza Impact Analysis (2018-2019)

### Overview  
This project investigates the spatial and social patterns of influenza transmission in the U.S. during the 2018-2019 season using **ArcGIS Pro** and **Python**. It combines flu surveillance data, demographic data from the Census, and geospatial analysis tools to explore the potential role of multigenerational households in influencing flu positivity across states.

---

### Tools Used
- **ArcGIS Pro 3**  
- **Python** (Pandas, Matplotlib, Seaborn)  
- **Google Sheets** (for quick feature engineering)  
- **CDC FLUVIEW Data Portal**  
- **U.S. Census ACS Tables** (via [data.census.gov](https://data.census.gov))  

---

### Datasets
- **ILINet (CDC)**: ILI surveillance across states  
- **ICL NREVSS Clinical Labs (CDC)**: Lab-confirmed influenza data  
- **Multigenerational Households (ACS)**: Household structure statistics  
- **State Boundaries Shapefile (Census)**: For geospatial joins and visualization  

---

### Methodology
- Cleaned and preprocessed CDC datasets (removed missing values, engineered consistent flu week indicator).  
- Joined ILINet and Clinical data to U.S. States using geodatabases.  
- Aggregated season-level statistics.  
- Visualized using:
  - Choropleth maps  
  - Proportional symbol maps  
  - Hotspot analysis (Getis-Ord Gi*)  
- Built **Random Forest** model to test predictive capacity (poor result).  

---

### Key Findings
- Volume-based metrics (ILI cases, patients) **correlate strongly**.  
- Multigenerational household percentage has **weak correlation** with flu positivity.  
- **Southeastern U.S.** identified as flu hotspots (non-random clustering).  

---

### Limitations
- State-level granularity may hide local heterogeneity.  
- Only one flu season analyzed.  
- Environmental variables not fully integrated.  

---

### Future Work
- Add healthcare access and vaccination data  
- Conduct multi-season comparisons  
- Shift focus to county or zip-code level  

---

### Author  
**Nandhika Rajmanikandan** (MS Data Science),  
**Frank Ofusu** (MS Health Informatics)  
Michigan Technological University  

---

### License  
Open for educational and non-commercial use. **Attribution appreciated.**
