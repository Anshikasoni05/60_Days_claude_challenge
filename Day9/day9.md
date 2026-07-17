# Day 9 — 60-Day Claude Challenge

## Task
Build an MVP application using Claude, then enhance it with a second, more advanced prompt — and compare the two versions.

## Project: NutriScope — Nutrient Intelligence Dashboard

### Prompt 1 — MVP
Asked Claude to build a single-file HTML nutrition tracker (**NutriScope**) with:
- Profile inputs (age, gender, height, weight, activity level, dietary preference)
- Food logging against a 20-food database
- Calculated energy, macro, and micronutrient targets
- A dashboard (energy ring, macro chart, deficiency/excess lists, nutrient table)
- Basic food-based recommendations
- Premium dark SaaS UI, mobile responsive, Chart.js, no backend

**Result:** a fully working single HTML file — no frameworks, no server, opens directly in a browser.

### Prompt 2 — Enhancement
Asked Claude to upgrade the MVP with:
- CSV upload for bulk food logging
- 40 additional foods (60 total database)
- 4 new micronutrients: Magnesium, Zinc, Potassium, Vitamin A
- A 2-day meal planner (Breakfast/Lunch/Snacks/Dinner slots, per-day totals vs targets)
- A Risk Analysis tab (flags patterns like anemia risk, bone density risk, cardiovascular risk)
- An educational disclaimer + nutrition data sources section
- Two new charts: calorie-source doughnut, micronutrient coverage radar
- Advanced recommendations: nutrient pairing (e.g. iron + vitamin C for absorption), risk-based priority suggestions

**Result:** a significantly more capable version, still a single HTML file, still zero backend.

## MVP vs Enhanced — Comparison

| Aspect | MVP | Enhanced |
|---|---|---|
| Food database | 20 foods | 60 foods |
| Nutrients tracked | 10 | 14 (+ Mg, Zn, K, Vitamin A) |
| Food entry | Manual only | Manual + CSV upload |
| Planning | Today's log only | 2-day meal planner |
| Analysis | Deficiency/excess lists | + Risk Analysis with severity levels |
| Charts | Energy ring, macro bar | + Calorie doughnut, micronutrient radar |
| Recommendations | Add/swap/portion | + Nutrient pairing, risk-based priority |
| Trust/transparency | — | Disclaimer + nutrition data sources |

## Key Learnings
- A single, well-structured prompt can produce a genuinely usable MVP — but the second pass is where a tool becomes trustworthy: sources, disclaimers, and risk context turned a calculator into something that reads like a real product.
- Expanding a data-heavy app (food database, nutrient targets) is mostly about disciplined data modeling — get the schema right once, and every new food/nutrient just slots in.
- Iterative prompting (build → enhance) is a much stronger workflow than trying to specify everything in one giant prompt.

## Files
- `nutriScope.html`
- EnhancedNutriScope.html`
-# Day 9 — 60-Day Claude Challenge

## Task
Build an MVP application using Claude, then enhance it with a second, more advanced prompt — and compare the two versions.

## Project: NutriScope — Nutrient Intelligence Dashboard

### Prompt 1 — MVP
Asked Claude to build a single-file HTML nutrition tracker (**NutriScope**) with:
- Profile inputs (age, gender, height, weight, activity level, dietary preference)
- Food logging against a 20-food database
- Calculated energy, macro, and micronutrient targets
- A dashboard (energy ring, macro chart, deficiency/excess lists, nutrient table)
- Basic food-based recommendations
- Premium dark SaaS UI, mobile responsive, Chart.js, no backend

**Result:** a fully working single HTML file — no frameworks, no server, opens directly in a browser.

### Prompt 2 — Enhancement
Asked Claude to upgrade the MVP with:
- CSV upload for bulk food logging
- 40 additional foods (60 total database)
- 4 new micronutrients: Magnesium, Zinc, Potassium, Vitamin A
- A 2-day meal planner (Breakfast/Lunch/Snacks/Dinner slots, per-day totals vs targets)
- A Risk Analysis tab (flags patterns like anemia risk, bone density risk, cardiovascular risk)
- An educational disclaimer + nutrition data sources section
- Two new charts: calorie-source doughnut, micronutrient coverage radar
- Advanced recommendations: nutrient pairing (e.g. iron + vitamin C for absorption), risk-based priority suggestions

**Result:** a significantly more capable version, still a single HTML file, still zero backend.

## MVP vs Enhanced — Comparison

| Aspect | MVP | Enhanced |
|---|---|---|
| Food database | 20 foods | 60 foods |
| Nutrients tracked | 10 | 14 (+ Mg, Zn, K, Vitamin A) |
| Food entry | Manual only | Manual + CSV upload |
| Planning | Today's log only | 2-day meal planner |
| Analysis | Deficiency/excess lists | + Risk Analysis with severity levels |
| Charts | Energy ring, macro bar | + Calorie doughnut, micronutrient radar |
| Recommendations | Add/swap/portion | + Nutrient pairing, risk-based priority |
| Trust/transparency | — | Disclaimer + nutrition data sources |

## Key Learnings
- A single, well-structured prompt can produce a genuinely usable MVP — but the second pass is where a tool becomes trustworthy: sources, disclaimers, and risk context turned a calculator into something that reads like a real product.
- Expanding a data-heavy app (food database, nutrient targets) is mostly about disciplined data modeling — get the schema right once, and every new food/nutrient just slots in.
- Iterative prompting (build → enhance) is a much stronger workflow than trying to specify everything in one giant prompt.

## Files
- `NutriScope-MVP.html`
- `NutriScope-Enhanced.html`
  
