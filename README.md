# FPT Group Financial Strategy & Capital Allocation Analysis (2018–2022) 📈

## 📌 Business Context & Objective
The 2018–2022 period was a transformative era for FPT Group, marked by aggressive digital transformation amidst macroeconomic volatility. This project delivers a comprehensive Power BI framework to evaluate FPT’s financial health, decoding the strategic balance between **"Hyper-growth"** (Technology expansion) and **"Financial Safety"** (Liquidity management).

## 🎯 Project Scope
- **Data Modeling:** Built a robust model to track 15+ core financial KPIs.
- **Capital Analysis:** Visualized capital structure, working capital efficiency, and fixed asset turnover.
- **Risk Assessment:** Evaluated financial leverage and solvency ratios over a 5-year horizon.

## 🛠 Tech Stack & Skills
- **Tool:** Power BI (Data Modeling, Data Visualization).
- **Advanced DAX:** Engineered complex measures for Time Intelligence and Financial Ratios.
- **Business Acumen:** Financial Statement Analysis & Strategic Assessment.

## 💡 Strategic Insights & Data Storytelling
### 1. The "Asset-Light" Competitive Advantage
- **Insight:** Analysis reveals that working capital consistently accounts for ~60% of total assets. 
- **Strategic Value:** This highlights FPT's "Asset-light" model, allowing for high operational agility and rapid cash flow pivot during the pandemic.

### 2. Strategic CAPEX Trade-offs
- **Insight:** Identified a slight decline in fixed asset efficiency (from 0.24 to 0.22). 
- **Strategic Value:** This was a **deliberate trade-off**, as FPT aggressively invested in long-term infrastructure (Data Centers, Campuses) to secure future technological leadership.

### 3. Financial Leverage & Liquidity
- **Insight:** FPT effectively utilized leverage to scale operations while maintaining a safe Current Ratio of 1.3 in 2022.
- **Strategic Value:** Demonstrates a disciplined approach to funding growth through debt without compromising short-term solvency.

## 🚀 Technical Highlight (DAX)
Calculated dynamic Year-over-Year (YoY) growth for Revenue using:
```dax
Revenue YoY % = 
VAR PrevYearRevenue = CALCULATE([Total Revenue], SAMEPERIODLASTYEAR('Date'[Date]))
RETURN 
DIVIDE([Total Revenue] - PrevYearRevenue, PrevYearRevenue, 0)
