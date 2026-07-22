# Day 17 — Vehicle Cost Analysis Dashboard (E85 Economics Deep Dive)

## 🎯 Task
Built a fully self-contained HTML dashboard analyzing fuel cost, CO₂ emissions, maintenance cost, and E85 (Flex-Fuel) economics for a **Toyota Fortuner (Diesel, 3 years old, 1000 km/month, mixed city+highway use)**, using a 52-row CSV dataset spanning 5 fuel types: Petrol (E20), Diesel, CNG, Electric (EV), and E85 (Flex-Fuel).

## 🧠 Approach
- Prompted Claude with a detailed spec: exact formulas, layout, chart types, and theme (dark navy glassmorphism UI).
- All calculations run live in embedded JavaScript from the raw CSV rows — no hardcoded numbers.
- Charts built in pure SVG (no libraries/CDNs): animated bar chart, doughnut chart with hover tooltips, multi-line chart with a vehicle-age marker, and an animated gauge.

## 📊 Key Findings

**Cost per km by fuel (avg):**
| Fuel | Cost/km | CO₂/km | Maintenance/km | Refuel Time |
|---|---|---|---|---|
| Electric (EV) | ₹1.75 | 0.091 kg | ₹0.23 | 45 min |
| CNG | ₹3.32 | 0.125 kg | ₹0.66 | 8 min |
| Diesel (selected) | ₹4.67 | 0.179 kg | ₹1.00 | 5 min |
| Petrol (E20) | ₹6.15 | 0.171 kg | ₹0.47 | 5 min |
| E85 (Flex-Fuel) | ₹6.37 | 0.070 kg | ₹0.46 | 5 min |

**E85 Paradox:**
- Pump price saving vs Petrol: **18.0%** (E85 is cheaper per litre)
- Running cost penalty vs Petrol: **+3.6%** (but costs more per km due to lower mileage)
- Break-even fuel price: **₹79.11/unit** for E85 to match Petrol's cost/km
- **E85 Score: 5.7/10** — wins big on CO₂ (lowest of all fuels) and refuel time, but loses on cost/km, since its mileage disadvantage outweighs the pump-price saving.

**Diesel (this vehicle's fuel):**
- Highest maintenance cost/km (₹1.00) and highest CO₂/km (0.179 kg) of all 5 fuels.
- Best suited for high-mileage mixed city+highway driving needing torque/range — matches this vehicle's usage pattern.
- Vehicle age bucket "Mid-life (3–5y)" shows the lowest average cost/km (₹4.09) across the dataset — favorable timing for this 3-year-old vehicle.

## 💡 Learnings
- The "obvious" E85 pump-price saving is misleading in isolation — the real economics only show up once mileage/efficiency is folded into a cost-per-km comparison, which is why the break-even calculation matters more than the sticker saving.
- Normalizing multiple weighted metrics (cost, CO₂, refuel time, maintenance) into one score requires picking a fair baseline (min/max across all fuel types) rather than arbitrary thresholds — small design choice, big effect on the final number.
- Building all SVG charts from scratch (bar, doughnut, multi-line, gauge) without any charting library reinforced how much boilerplate (scaling, path arcs, tooltips) is normally hidden by libraries like Chart.js/Recharts.

## 📎 Attachments
- `toyota-fortuner-fuel-dashboard.html` — full interactive dashboard
- Screenshots of KPI cards, charts, and fuel comparison cards
<img width="1083" height="861" alt="image" src="https://github.com/user-attachments/assets/77b4bd2b-5dbb-4208-87b3-e3b172136e80" />
<img width="1040" height="855" alt="image" src="https://github.com/user-attachments/assets/5f03b49e-8285-49d1-82bd-47fdc738b30a" />
<img width="1028" height="769" alt="image" src="https://github.com/user-attachments/assets/b6e65e2a-0ba8-4c87-9a73-0567c06e0051" />


---
#60DayClaudeChallenge · Day 17 · @Anthropic @ABTalksOnAI @AnilBajpai
