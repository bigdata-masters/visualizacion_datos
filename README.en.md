<p align="right">
  <a href="./README.md">
    <img alt="Español" src="https://img.shields.io/badge/ES-Español-blue">
  </a>
  <a href="./README.en.md">
    <img alt="English" src="https://img.shields.io/badge/EN-English-lightgrey">
  </a>
</p>

# Data Visualization - Analysis of the Leading Causes of Death Worldwide

## Description
This dashboard was designed to visualize the **main causes of death worldwide**, considering only those that represent **0.5% or more of total global deaths**.

Causes with lower incidence were grouped under a category named **“Others”**, allowing for a cleaner and more comparative representation.  
The main goal was to create a **clear, readable, and minimalist visualization** that enables quick interpretation of the data.

## 🧰 Tools Used
<code><img title="Power BI" alt="power bi" width="40px" src="https://raw.githubusercontent.com/microsoft/PowerBI-Icons/f1d4dd6cd52338a186f58bc29c437f64cf6b327b/SVG/Power-BI.svg" /></code>


## Dataset
**Main variables:**
- **Cause of death or injury** → Cause of death or injury.  
- **Percent of total deaths** → Percentage of total deaths (range 0–1).  
- **Deaths annual % change** → Annual percentage change in deaths (range -1 to 1).

## Analysis and Design Process

1. Filtering of Relevant Causes
- Included only causes of death contributing **≥ 0.5% of total global deaths**.  
- All other causes were grouped under an **“Others”** category using a conditional measure (`IF` + `GROUP BY`).

2. Main Visualization, **Scatter plot** representing:  
  - **X-axis:** Annual change in deaths (`Deaths annual % change`).  
  - **Y-axis:** Percentage of total deaths (`Percent of total deaths`).  
  - **Labels:** Cause of death.

3. Visual Comparison
    - Allows for quick identification of which causes account for higher proportions and whether they show an **upward or downward trend**.  
    - Neutral colors were used to maintain visual cleanliness and highlight **positive or negative variations**.

4. Interactivity and Accuracy
    - Added **tooltips** to display exact percentage and annual variation values.  
    - Axis scales were adjusted to match the actual data range, avoiding visual distortion.

## Results and Insights
The **main global causes of death** identified were:
- **Ischemic heart disease**  
- **Stroke**  
- **Chronic obstructive pulmonary disease**

Identified **positive and negative annual variation patterns**:
- Causes such as **respiratory infections** and **diarrheal diseases** showed a decline.  
- Some **non-communicable diseases** (e.g., cancer or Alzheimer’s) continued to show slight growth.  
- The **“Others”** category groups causes with very low incidence (< 0.5%).

<p align="center">
  <img src="/assets/causes_of_death.png" alt="causes_of_death" />
</p>
<p align=center><em>Figure 1. Causes of death</em></p>

## ⚙️ Authors:
- [Alonso Ismael Camarena](https://www.linkedin.com/in/camarenaai/)
- [Erick Martinez Blas](https://www.linkedin.com/in/erick-martinez-blas/)