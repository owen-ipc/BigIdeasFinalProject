# BigIdeasFinalProject: Finding the Best Neighborhood in Pittsburgh

## Project Overview
Our final project evaluates Pittsburgh neighborhoods to determine the overall "best" neighborhood to live in by analyzing three metrics: **public safety**, **firearm safety**, and **environmental richness**. All datasets are sourced from the City of Pittsburgh via the Western Pennsylvania Regional Data Center.

---

## Team Members & Datasets
* **Andrew Snyder** – *Police Arrest Data*
* **Danny Wan** – *Pittsburgh City Trees Data*
* **Owen Arnold** – *Firearm Seizures Per Capita*

---

## Side-by-Side Dataset Comparison

| Metric / Feature | Police Arrests | City Trees | Firearm Seizures |
| :--- | :--- | :--- | :--- |
| **Core Measurement** | Total police arrests per neighborhood over a 2-year period. | Total number of city-maintained trees per neighborhood. | Firearm seizures per 1,000 residents normalized using 2020 Census population. |
| **Guiding Assumption** | Fewer arrests indicate lower crime rates and a way more peaceful community. | Higher tree counts indicate more greener, healthier, and more aesthetically pleasing neighborhoods. | Fewer firearm seizures per capita indicate safer residential environments. |
| **Data Cleaning** | Dropped null neighborhoods, removed outside-city records, and standardized neighborhood spelling. | Filtered out missing neighborhood values and invalid entries. | Dropped missing neighborhood rows, merged with 2020 population data, and filtered out extreme per-capita outliers. |
| **Best Neighborhoods** | **Mt. Oliver Neighborhood**, followed by Troy Hill-Herrs Island and Mt. Oliver Boro. | **Squirrel Hill South** with 5,073 trees, followed by Highland Park with 2,941 and Squirrel Hill North with 2,083. | **Swisshelm Park**, **Squirrel Hill North**, **North Oakland**, and **Shadyside**. |
| **Worst Neighborhoods** | **Central Business District**, followed by South Side Flats and Carrick. | **Hays** with 1 tree, followed by South Shore with 2 and Glen Hazel with 2. | **Homewood South**, **Homewood West**, and **Larimer**. |

---

## Key Insights & Cross-Dataset Synthesis

1. **The Impact of Foot Traffic vs. Residential Living**:
   * In the **Police Arrests** dataset, the **Central Business District** ranked worst due to high arrest counts, which is heavily skewed by dense commercial activity and daily visitors rather than residential population. However, it still ranked in the top 10 for **City Trees** with 1,002 trees.
2. **Population Normalization Matters**:
   * While raw counts work well for physical infrastructure like trees, normalizing **Firearm Seizures** per 1,000 residents prevents large-population neighborhoods from being unfairly penalized.
3. **Top Overall Contenders**:
   * **Squirrel Hill North** stands out as a top performer across multiple metrics - ranking 3rd best for City Trees and 2nd best for lowest Firearm Seizures per capita.
   * **Swisshelm Park** and **Regent Square** also perform consistently well in both low arrest counts and low firearm seizures.
   * **Squirrel Hill South** dominates in the green coverage while maintaining very low firearm seizure rates, making the Squirrel Hill area one of the strongest overall communities in Pittsburgh.

---

## How to Run the Notebooks
1. Clone this repository to your local machine.
2. Ensure Python 3, `pandas`, and `matplotlib` are installed.
3. Open any of the `.ipynb` files in JupyterLab or Jupyter Notebook and run all cells.
