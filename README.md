# 📊 Startup Failure Analysis: Uncovering Business Risks & Survival Patterns
By Damola Adediran

---

## Project Overview
This project analyzes **startup failures across multiple industries** to identify **key risk factors, failure reasons, and their impact on survival time**. Using **Python, Pandas, Seaborn, Matplotlib, and Scipy**, we perform **statistical hypothesis testing** and **data visualization** to uncover actionable insights for **entrepreneurs, investors, and policymakers**.

## Key Objectives
* Identify **which failure reasons are most common in each industry**.  
* Test whether **certain failure reasons impact how long startups survive**.  
* Evaluate whether **external factors (Regulatory Pressure, Trend Shifts) accelerate failure**.  
* Use **statistical tests (Chi-Square, Kruskal-Wallis, Mann-Whitney U)** to derive insights.  
* Create **data visualizations (bar charts, box plots, violin plots, heatmaps)** to showcase patterns.  

---

## Data Description
The dataset consists of **failed startups from various industries** with recorded failure reasons, funding status, and survival time.

### **Key Columns**
- **Sector** → Industry category of the startup.
- **Years in Business** → Number of years before the startup failed.
- **Failure Reasons (Binary 0/1)**:
  - **Competition** → Lost to market rivals.
  - **No Budget** → Ran out of funding.
  - **Monetization Failure** → Could not generate revenue.
  - **Regulatory Pressure** → Legal restrictions or government regulations caused failure.
  - **Trend Shifts** → Market trends changed, reducing demand.

---

## Hypothesis Testing & Statistical Methods
### **Hypothesis 1: Are Failure Reasons Industry-Specific?**
* **Test Used:** Chi-Square Test  
* **Result:** **Failure reasons significantly depend on industry (p-value = 0.00000).**  
* **Insight:** **Tech startups fail due to Giants & No Budget; Finance struggles with Regulations.**

### **Hypothesis 2: Does Competition Lead to Longer Survival?**
* **Test Used:** Kruskal-Wallis Test  
* **Result:** **No significant difference in survival time based on failure reason (p-value = 0.46405).**  
* **Insight:** **Failure reason alone does not determine how long a startup survives.**

### **Hypothesis 3: Do External Factors (Regulation & Trend Shifts) Accelerate Failure?**
* **Test Used:** Kruskal-Wallis Test  
* **Result:** **No significant difference in survival time (p-value = 0.95864).**  
* **Insight:** **Regulatory Pressure & Market Trends do not significantly shorten startup survival.**

---

## Data Visualizations
* **Failure Reasons by Sector** → Stacked bar chart showing the most common reasons per industry.  
* **Survival Time by Failure Reason** → Box plot comparing **Competition, Monetization Failure, No Budget**.  
* **Survival Distribution for Regulations & Trend Shifts** → Violin plot showing the lifespan patterns.  
* **Heatmap of Sector vs. Failure Reasons** → Visualizes **which industries suffer most from specific risks**.  
