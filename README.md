# Online-Retail-Revenue-Expansion-Analysis
# 🛍️ Online Retail Revenue & Expansion Analysis
### Tata Data Science Virtual Experience Program — Forage

An end-to-end data analytics project simulating a real consulting assignment for a UK-based online retail store. Analyzed one year of transaction data to uncover revenue drivers, key markets, top customers, and data-backed international expansion opportunities.

---

## 📌 Business Problem

The CEO and CMO of an online retail store wanted answers to four strategic questions:

1. How did monthly revenue trend through 2011, and what should we plan for?
2. Which countries (outside the UK) generate the most revenue and order volume?
3. Who are our most valuable customers, and how concentrated is our revenue?
4. Where should we expand next, based on existing demand?

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python (Pandas) | Data cleaning, transformation, aggregation |
| Matplotlib / Seaborn | Line charts, bar charts, column charts |
| Geo-visualization (map chart) | Country-wise demand mapping |
| Jupyter Notebook | Analysis environment |

---

## 📊 Dataset

| Property | Detail |
|---|---|
| Source | UCI Online Retail Dataset |
| Raw Rows | 5,41,909 transactions |
| Clean Rows | 5,31,283 transactions |
| Rows Removed | 10,626 (returns, cancellations, pricing errors) |
| Period | December 2010 – December 2011 |
| Geography | UK + 37 other countries |

---

## 🔍 Methodology

### Phase 1 — Data Cleaning
- Removed rows with `Quantity < 1` (returns and cancelled orders)
- Removed rows with `UnitPrice < 0` (data entry errors)
- Dropped 10,626 invalid rows, retained 5,31,283 clean transactions
- Engineered a new `Revenue` column = `Quantity × UnitPrice`

### Phase 2 — Exploratory & Business Analysis
- Monthly revenue trend analysis (2011)
- Country-wise revenue and quantity ranking (excluding UK)
- Customer-level revenue concentration analysis
- Geographic demand mapping for expansion planning

### Phase 3 — Visualization & Storytelling
- Line chart — monthly revenue trend
- Bar chart + line overlay — top 10 countries by revenue and quantity
- Column chart — top 10 customers by revenue
- Map chart — global demand distribution (excluding UK)

---

## 📈 Key Findings

### Finding 1 — Strong Seasonal Revenue Spike
Revenue held steady between **£5.2–7.7 lakh/month** through August 2011, then surged sharply:

| Month | Revenue |
|---|---|
| September 2011 | £10.6 lakh |
| October 2011 | £11.5 lakh |
| November 2011 | £15.1 lakh (peak) |

This confirms a clear **pre-Christmas demand cycle**, requiring advance planning for stock, staffing, and marketing from September onward. (December appears artificially low — the dataset ends December 9.)

### Finding 2 — Top 5 International Markets
Excluding the UK, revenue is concentrated in a handful of key markets:

| Rank | Country | Revenue |
|---|---|---|
| 1 | Netherlands | £2,85,446 |
| 2 | Ireland | £2,83,454 |
| 3 | Germany | — |
| 4 | France | — |
| 5 | Australia | — |

Revenue drops sharply after these five, marking them as the business's core international markets.

### Finding 3 — High Customer Revenue Concentration
- **Customer 14646** — £2,80,206 (top customer)
- **Customer 18102** — £2,59,657 (second)
- **Top 10 customers combined** — over £15 lakh, ~17% of total customer revenue

This level of concentration means losing even a few top accounts would materially impact revenue — prioritizing retention for this segment is critical.

### Finding 4 — Expansion Opportunity
A demand map (excluding UK) shows the strongest non-UK demand clustered in nearby Europe:

- **Netherlands, Ireland, Germany, France** — each over 1,00,000 units
- **Australia** — 84,209 units (best non-European market)

---

## ✅ Recommendations

1. **Expand first in the Netherlands, Ireland, Germany, and France** — demand is already proven, and delivery logistics are faster and cheaper due to proximity.
2. **Test Australia** as the next market beyond Europe, given its standout demand outside the continent.
3. **Protect peak season performance** — plan inventory, staffing, and marketing campaigns well ahead of September–November.
4. **Prioritize top customers** with dedicated service and personal account management, given their outsized revenue contribution.

---
** Skills learned in this simulation
Dashboard Development, Data Analysis, Data Analytics, Data Cleaning, Data Interpretation, Data Presentation, Data Visualization, Effective Communication, Visual Basic

## 🎯 Conclusion

The business is healthy but carries concentration risk — it depends heavily on the UK market, one seasonal peak, and a small group of high-value customers. The clearest path to sustainable growth is deepening penetration in already-proven nearby European markets while safeguarding the revenue base that currently exists.

---

## 👤 About This Project

Completed as part of the **Tata Data Science Virtual Experience Program** on Forage — a simulated consulting assignment applying real-world data cleaning, business analysis, and stakeholder-focused storytelling.
