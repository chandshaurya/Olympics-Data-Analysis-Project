#- 🏅 Olympics Data Analysis Project

## 📌 Project Objective
The goal of this project is to analyze Olympic Games results and uncover insights into athlete performance, country participation, medal distribution, and event-level trends.  
This project demonstrates data cleaning, exploratory data analysis (EDA), and visualization skills using **Python (pandas, matplotlib, seaborn)**.

---

## 📂 Dataset
- **Source**: Olympic Results dataset ( 4 CSV )  
- **Rows**: ~220K  
- **Period**: 1896-2022

---

## 🔄 Workflow
1. **Data Loading**: Imported CSV file using pandas.  
2. **Data Cleaning**: Treated null values, standardized text, and adjusted datatypes.  
3. **EDA (Exploratory Data Analysis)**:  
   - Distribution of medals by country and athlete.  
   - Participation trends across years and sports.  
   - Gender and event-level analysis.  
4. **Visualization**: Plotted insights using bar charts, heatmaps, and time-series trends.  
5. **Insights**: Summarized findings for performance trends and country dominance.

---

## 🧹 Data Cleaning
- Replaced `FALSE` values with `NaN` and applied column-wise strategies:
  - `medal_type`: Filled missing with `"No Medal"`.  
  - `athletes` & `athlete_full_name`: Filled missing with `"Team"` for team events.  
  - `rank_equal`: Filled missing with `0` (no tie).  
  - `rank_position`: Filled missing with `0` (no rank).  
  - `country_code`: Replaced nulls with `"UNK"`.  
  - `athlete_url`: Replaced nulls with `"No URL"`.  
  - `value_unit`, `value_type`: Replaced nulls with `"N/A"`.  
- Standardized text columns (title case, removed extra spaces).  
- Converted categorical fields (`medal_type`, `country_name`, `event_title`) into **category** datatype.  
- Removed duplicates (reduced rows from 162,804 → 162,688).

---

## 📊 Exploratory Data Analysis (EDA)
Key analyses performed:
- **Medal Distribution**: Top countries by Gold, Silver, Bronze, and total medals.  
- **Participation Trends**: Number of athletes and countries per Olympic edition.  
- **Event-Level Insights**: Which disciplines generate the most medals.  
- **Gender Analysis**: Female vs. male participation over time.  
- **Performance Trends**: Identified how certain nations dominate specific sports.  

---

## 📈 Summary & Insights
- A small number of countries consistently dominate medal tables (e.g., USA, China, Russia).  
- Participation has steadily increased over the years, with **more female athletes joining in recent editions**.  
- Team events contribute significantly to medal counts but often lack detailed athlete-level information.  
- KPIs like **rank_position** and **medal_type** are strong indicators for analyzing competitiveness.  
- Data cleaning ensured reliable insights by converting `"FALSE"` placeholders into meaningful replacements.  

---

## 🛠️ Tech Stack
- **Language**: Python  
- **Libraries**: pandas, numpy, matplotlib, seaborn  
- **Tools**: Jupyter Notebook  

---


