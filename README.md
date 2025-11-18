# Electric-Vehicles-Market-Size-Analysis-Python

##  Project Objective

To analyze a real-world EV dataset and uncover insights about pricing, battery performance, energy consumption, and manufacturer differences.  
The project also includes hypothesis testing and a recommendation engine to support customer purchase decisions.

---

#  Dataset Overview

**Dataset:** `FEV-data-Excel.xlsx`  
Contains vehicle specifications such as:

- Make, Model, Full Name  
- Minimal Price (PLN)  
- Battery Capacity (kWh)  
- Electric Range (WLTP km)  
- Engine Power (KM)  
- Maximum Torque (Nm)  
- Drive Type (FWD/RWD/AWD)  
- Boot Capacity, Load Capacity  
- Maximum Speed  
- Charging Power  
- Energy Consumption (kWh/100 km)  
- Dimensions & Weight  
- Seats, Doors, Tire Size  

This dataset provides a holistic view of EV performance and pricing.

---

#  Tasks Performed

## **1️⃣ Filter EVs by Customer Requirements**
A customer wants:
- **Budget ≤ 350,000 PLN**
- **Minimum Range ≥ 400 km**

I filtered EVs meeting these conditions, grouped them by **manufacturer (Make)**, and calculated each manufacturer's **average battery capacity**.

---

## **2️⃣ Outlier Detection in Energy Consumption**
Using statistical methods (IQR/Z-score), I identified EVs with unusually high or low **mean energy consumption** (kWh/100 km).  
These outliers represent exceptionally efficient or inefficient EVs.

---

## **3️⃣ Relationship Between Battery Capacity & Range**
- Created a scatter plot to visualize the relationship  
- Analyzed how battery size influences real-world range  
- Highlighted strong positive correlation insights  
- Identified which models provide the best range-to-capacity efficiency  

---

## **4️⃣ EV Recommendation Class (OOP Project Component)**
Built a Python **Recommendation Class** where users can input:

- Budget  
- Desired Range  
- Battery Capacity  

The class returns the **top 3 EVs** matching their criteria.  
This helped link analysis with practical, user-friendly automation.

---

## **5️⃣ Hypothesis Testing — Tesla vs Audi**
Conducted a **two-sample t-test** to check whether:

**"Tesla and Audi have the same average engine power."**

Using `ttest_ind` from `scipy.stats`, I:
- Compared mean engine power  
- Evaluated statistical significance  
- Provided business insights based on test results  
- Suggested which brand delivers superior performance  

---

# 📊 Tools & Libraries Used
- **Python**
- **Pandas** — data cleaning & transformation  
- **NumPy** — numeric operations  
- **SciPy** — t-test & statistical analysis  
- **Matplotlib / Seaborn** — visualizations  
- **OOP (Classes)** — custom recommendation engine  

---

# 📈 Key Insights
- Several EVs deliver high range within the budget segment  
- Battery capacity strongly influences range  
- Energy consumption varies widely, with some models being clear outliers  
- Tesla generally shows stronger engine performance compared to Audi  
- The EV recommendation system helps customers instantly find suitable options  

---


