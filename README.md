# CSC8626 – Data Visualization Coursework Dashboard (Power BI)

## 📌 Overview
This project is created for the **CSC8626 – Data Visualization** coursework.  
The dashboard is designed to support exploration of **UK housing energy efficiency and carbon dioxide emissions** using interactive Power BI visualizations.

The solution focuses on enabling users to:
- Explore **carbon dioxide emission patterns geographically**
- Understand **energy efficiency evolution over time**
- Discover **relationships between multiple variables** such as:
  - property type
  - location (UK regions / local authority districts)
  - energy efficiency (EPC bands)
  - tenure
  - carbon dioxide emissions

---

## 🎯 Coursework Tasks Addressed

### 1) 📍 Location Task
**Question:**  
How does the visualization allow users to access the spread of carbon dioxide emission across the UK based on property type?

**Implementation:**
- Uses **ArcGIS Map for Power BI** to display a choropleth map of the UK.
- Geographic boundaries are plotted using **Local Authority District name**.
- CO₂ emission magnitude is encoded using a **sequential colour scheme**:
  - light shades → lower median CO₂ emissions
  - darker shades → higher median CO₂ emissions
- Users can filter by **property type** (e.g., Detached, Flats and maisonettes).
- The map supports visual information seeking:
  - Overview → Zoom/Filter → Details-on-demand
- Interactive filtering enables users to:
  - view national patterns
  - identify hotspot local authorities
  - explore breakdowns via linked charts

---

### 2) 🕒 Time Task
**Question:**  
How does the visualization allow users to understand the evolution of energy efficiency based on property type and location?

**Implementation:**
- **Donut chart** provides a clear summary of:
  - total counts
  - percentages by property type
- **Line chart** updates dynamically based on donut selection.
- Selecting a property type (e.g., “Detached”) instantly filters the line chart to show how EPC-related values change over time.
- Geographic or region-based filtering enables users to explore energy efficiency trends at a local level.

---

### 3) 🔗 Multi-dimensional Data Task
**Question:**  
How does the visualization allow the user to identify correlations among at least three of:
property type, tenure, location, energy efficiency, carbon dioxide emission?

**Implementation:**
The dashboard enables correlation detection using coordinated multi-chart interactions:

- A bar chart such as **"Count of EPC Band by Country or region name"** supports comparison of energy efficiency distribution across regions.
- Selecting a region (e.g., London) filters other visuals, helping users evaluate:
  - which property types dominate specific EPC band patterns
  - how location influences efficiency outcomes
- If CO₂ and tenure are included in the filtered selection, users can further inspect:
  - tenure-property-location patterns
  - relationship between EPC and emissions

This multi-visual interaction supports deeper analytic exploration and pattern detection.

---

## 📊 Dashboard Visual Components

The dashboard includes a combination of visualisations, including:

- **ArcGIS Choropleth Map**
  - Median CO₂ emission by local authority district
- **100% Stacked Bar Chart**
  - property mix distribution across local authorities
- **Clustered / Stacked Bar Charts**
  - EPC distribution across UK regions
- **Donut Chart**
  - property type composition
- **Line Chart**
  - tenure / energy efficiency trends over time
- **KPI Card**
  - summary metric showing total CO₂ emission (e.g., 5.59K)

---

## 🎨 Visualization Principles Applied

### ✅ Use of Colour
Colour is applied to improve readability and effectiveness:

- **Categorical colours** distinguish property types clearly in the donut chart.
- **Sequential colour scheme** (light to dark purple) is used on the map to communicate CO₂ emission magnitude.
- High colour contrast against neutral background reduces confusion and increases legibility.
- KPI (5.59K) is displayed using prominent text for emphasis.

---

### ✅ Graphic Design Principles
The dashboard uses key design principles for clarity:

- **Grid layout** separates visuals cleanly.
- **Consistent typography** builds visual hierarchy.
- **Contrast** ensures data is the focus.
- Structured arrangement reduces cognitive overload and supports quick scanning.

---

### ✅ Interaction
Interactivity improves exploration and interpretation:

- Clicking on regions, property types, or map areas cross-filters the rest of the visuals.
- Users can move from:
  - high-level overview
  → regional focus
  → property breakdown
  → EPC/emission interpretation

This improves decision support and analytical depth.

---

### ✅ Use of Text and Legends
Text elements improve comprehension:

- Clear chart titles define context and reduce ambiguity.
- Axis labels indicate scale and measure correctly.
- Legends map colours to categories (e.g., property types).
- KPI text emphasizes the most important metric.

---

## 🛠️ Tools & Technologies

- **Power BI**
- **ArcGIS for Power BI**
- **Power Query** (data cleaning and transformation)
  - flattening tables
  - splitting columns
  - preparing categorical dimensions

---

## 📌 Key Insights Enabled by the Dashboard
This dashboard supports:
- Identifying regional CO₂ emission hotspots
- Comparing emissions by property type
- Exploring relationships between:
  - EPC band distribution
  - region / local authority
  - property type composition
  - tenure trends
- Supporting policy analysis and intervention planning

---

## 👤 Author
**Nisarga**  
Module: CSC8626 – Data Visualization  

---

## 📜 License
This project is created for academic coursework submission only.

