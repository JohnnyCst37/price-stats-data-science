<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=1f77b4&height=120&section=header"/>

[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=1f77b4&size=35&center=true&vCenter=true&width=1000&lines=SUPERMARKET+PRODUCT+ANALYSIS+IN+CHILE;PRICE+STATISTICS+BY+CATEGORY+AND+BRAND;Using+Mean,+Median,+and+Standard+Deviation;WITH+GRAPHS+AND+MAPS;WELCOME+TO+MY+PORTFOLIO!)](https://git.io/typing-svg)

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Graphical%20Visualization-blue?logo=matplotlib)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---


## 📑 Summary

- [Objective](#objective)
- [Technologies](#technologies-used)
- [Project Structure](#project-structure)
- [Statistical Analysis](#statistical-analysis)
- [Chart Examples](#chart-examples)
- [Possible Insights](#possible-insights)
- [How to Run](#how-to-run)
- [Dataset](#dataset-it-is-recommended-to-use-a-virtual-environment)
- [Author](#author)

---

# Comparative Analysis — Regular Price vs. Unit Price

This repository contains an exploratory analysis comparing **Regular Price (R$)** and **Unit Price** of supermarket products, with emphasis on variations across categories.  
The analysis was conducted using **Python**, leveraging data manipulation and visualization libraries.

---

## Objective

Evaluate pricing strategies and dispersion, identifying categories with the greatest impact and significant variation, highlighting:

- Products with the highest price fluctuation  
- Impact on specific categories such as **dairy** and **beauty & personal care**  
- Statistical distribution and behavior (mean, median, and standard deviation) by category

---

## Technologies Used

- **Python 3.13**
- **Jupyter Notebook** (recommended for interactive analysis)
- **Development Environments**: PyCharm / VSCode
- **Libraries**:
  - `pandas` — data manipulation
  - `numpy` — numerical operations
  - `matplotlib.pyplot` — static visualizations
  - `seaborn` — statistical plots
  - `plotly.express` — interactive charts and maps

---

## Project Structure

```
price-analysis-chile/
├── .git/                          # Git version control metadata
├── .ipynb_checkpoints/            # Auto-saved checkpoints from Jupyter
├── data/
│   └── raw/                       # Raw dataset files (e.g., CSV)
├── docs/                          # Documentation and interactive assets (e.g., treemap.html)
├── img/                           # Exported chart images and visualizations
├── notebooks/
│   ├── price_analysis.ipynb       # Main analysis notebook
│   └── data_scientist_study.ipynb # Legacy notebook for comparison and study
├── .gitignore                     # Git ignore rules for unnecessary files
├── README.md                      # Main project overview (English)
├── README_pt.md                   # Project overview in Portuguese
└── requirements.txt               # Python dependencies for the project
```

---

## Statistical Analysis

Price Analysis by Category
Overview

The Average Regular Price ($28.20) is higher than the Average Unit Price ($21.57), which indicates there's room for promotions and smaller packaging.

The high price dispersion (high standard deviation) suggests product heterogeneity, with different perceived value ranges.

### **General Statistics**
| Metric           | Regular Price (R$) | Unit Price |
|------------------|--------------------|------------|
| Mean             | 28.20              | 21.57      |
| Standard Deviation | 31.35            | 21.57      |
| Count (n)        | 813.000            | 813.000    |

---
Figure 1: General Statistics of Regular and Unit Prices. Note the large price dispersion in Regular Price, indicated by a standard deviation (31.35) higher than the mean (28.20), suggesting a high degree of product variety and price segmentation.

### **By Category — Regular Price (R$)**

| Category                    | Mean   | Median | Std. Dev. |
|-----------------------------|--------|--------|-----------|
| belleza-y-cuidado-personal | 29.20  | 21.79  | 21.63     |
| comidas-preparadas         | 39.55  | 37.40  | 13.22     |
| congelados                 | 30.21  | 29.54  | 19.04     |
| frutas                     | 17.24  | 11.95  | 16.39     |
| instantaneos-y-sopas       | 11.79  | 6.89   | 12.76     |
| **lacteos**                | **30.29** | **17.20** | **41.99** |
| verduras                   | 14.57  | 12.50  | 9.72      |

---

Figure 2: Statistical summary of regular prices by category. The notable difference between the mean ($30.29) and median ($17.20) for the 'lacteos' category, coupled with the highest standard deviation ($41.99), indicates a wide price range, likely driven by a few very expensive items or product types.

### **Comparison of Mean and Median Regular Price ($)**

| Category                     | Average Price (R$) | Median (R$) | Strategic Insight                                                                                       |
| ---------------------------- | ----------------- | ----------- | ------------------------------------------------------------------------------------------------------- |
| **Prepared Foods**           | 39.55             | 37.40       | Highest average ticket, **premium market**; consumers are willing to pay more.                          |
| **Frozen Foods**             | 30.21             | 29.54       | Stable values, low deviation; reliable category for predictable margins.                                |
| **Beauty & Personal Care**   | 29.20             | 21.79       | High dispersion → both basic and premium products. Opportunity for **audience segmentation**.            |
| **Dairy**                    | 30.29             | 17.20       | **Highest standard deviation (41.99)** → strong price volatility; **urgent portfolio and promotion review**. |
| **Fruits**                   | 17.24             | 11.95       | Low average value, focus on **volume and customer loyalty**.                                             |
| **Vegetables**               | 14.57             | 12.50       | Similar to fruits → low margins, but essential for driving customer traffic.                            |
| **Instant Foods & Soups**    | 11.79             | 6.89        | **Low-value category**, but can be used as a **promotional hook** to increase basket size.               |


---

## Chart Examples

> Below are some visualizations generated from the analysis (all images are stored in the `img/` folder):

### ✅ Price Dispersion — Boxplot Comparison
<img src="img/blox02.png" width="600"/>

### ✅ Price Distribution by Category — Interactive Treemap
<img src="img/treemap_interativo.png" width="400"/>

### ✅ Discount Distribution — Density Plot
To better understand how discounts are distributed across products, a density plot was generated using the difference between Regular Price and Unit Price.

Purpose
- Identify the most common discount ranges
- Detect skewness or concentration of discounts
- Highlight categories with aggressive pricing strategies
Methodology
The discount was calculated as:
discount = regular_price - unit_price

Then visualized using seaborn.kdeplot() to show the probability density of discount values.
Visualization
Below is the density plot showing the distribution of discounts across all products:

<img src="img/dens11.png" width="600"/>

---

## Possible Insights

- **Dairy products** show the largest difference between Regular and Unit Price.
- The **beauty & personal care** category has a tight median and standard deviation, indicating low dispersion and few outliers.
- Categories like **dairy** have high standard deviation, suggesting strong price variation.
- Unit Price tends to be more stable than Regular Price.

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/seu-usuario/price-analysis-chile.git

# Navigate to the project folder
cd price-analysis-chile

# (Optional) Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt
```

### Running the Analysis

- Open the main notebook:
  ```
  notebooks/analise_precos.ipynb
  ```

- For study and comparison purposes, explore:
  ```
  notebooks/Profissao Cientista de Dados_Extraindo_Médias.ipynb
  ```

---

## 📂Dataset (It is recommended to use a virtual environment)

The dataset is available in:

```
data/raw/
```

It is ready for analysis. To regenerate the charts, ensure all libraries are installed and run the notebooks via Jupyter.

---

## 👨‍💻Author

**Johnny Sorato Martins Fernandes**  
Business Consultant | Data & Visualization Specialist | Executive Director at Tutoreanos — Primavera do Leste Unit

---

## 🔖 Tags

`data-science`, `price-analysis`, `product-categories`, `descriptive-statistics`, `boxplot`, `discount-visualization`, `interactive-map`, `python`, `pandas`, `seaborn`, `plotly`

---
