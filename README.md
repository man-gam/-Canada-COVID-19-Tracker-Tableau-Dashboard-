# 🇨🇦 Canada COVID-19 Tracker (Tableau Dashboard)

An interactive Tableau dashboard to track **COVID-19 cases and deaths across Canadian provinces** (Jan 2020 – Jan 2023).  
The project highlights **data cleaning, modeling, and visualization skills**.

---

## 📊 Dashboard Preview
<img width="1573" height="789" alt="image" src="https://github.com/user-attachments/assets/c3eb7ed6-b5d9-4f48-8991-cc6ce40433b6" />


---

## 📂 Dataset
- **Source**: Publicly available COVID-19 dataset (Canada)
- **Duration**: Jan 1, 2020 – Jan 21, 2023
- **Key Fields**: Province, Cases, Deaths, Date, Repatriated Travellers

---

## 🎯 Objectives
- Integrated and modeled multiple datasets  
- Connected relationships between fact and dimension tables  
- Created calculated fields to fix running totals  
- Built sets to exclude irrelevant categories (Canada overall, Repatriated Travellers)  
- Designed bar graphs, trend lines, and maps for analysis  

---

## 🔎 Key Insights
- Ontario and Quebec reported the **highest number of cases** (over 1M each)  
- Alberta recorded **626K cases**, with a major spike in late 2021  
- Smaller provinces (Yukon, Nunavut, Northwest Territories) had fewer cases but still showed pandemic impact  
- Both cases and deaths followed **similar upward trends** across multiple waves  
- The last 7 days of the dataset reported **673 new cases** and **12 deaths**, proving the pandemic’s continued effect  

---

## ⚡ Challenges & Solutions
- **Challenge**: Tableau showed *Canada overall* and *Repatriated Travellers* in bar charts  
  - ✅ **Solution**: Used **Sets** to exclude those categories  

- **Challenge**: Dataset stored numbers as **running totals**, causing wrong sums in Tableau  
  - ✅ **Solution**: Created a **calculated field with MAX()** to extract correct daily totals  

- **Challenge**: Tableau summed running totals across dates  
  - ✅ **Solution**: Applied a **MAX(Date) calculation** for accurate daily reporting  

---

## 💡 Recommendations
- Automate dataset refresh for real-time updates  
- Add filters for **pandemic waves** (1st, 2nd, Omicron, etc.)  
- Include **per-capita metrics** (cases/deaths per 100K) for fairer comparisons  
- Add **annotations** for major events (lockdowns, vaccine rollouts)  

---

## 🚀 How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/covid19-canada-tracker.git
