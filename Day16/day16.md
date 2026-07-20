# Day 16 — Building a Custom Claude Skill: Stock Fundamental Analyzer

## Task
Turn a detailed stock-research prompt into a reusable **Custom Skill** in Claude, 
then test it across multiple Indian equities (Quick Take + Compare modes).

## What Was Built
A `stock-fundamental-research` skill that:
- Analyzes NSE/BSE-listed companies on fundamentals only (valuation, growth, 
  balance sheet health, ownership trends)
- Supports 5 modes: Quick Take, Deep Dive, Compare, Pros & Cons, Portfolio Fit
- Enforces hard rules: no buy/sell/hold calls, no fabricated data, mandatory 
  source citation, 2-source cross-check on key figures
- Ends every output with a fixed educational-use disclaimer

## Test Runs

**Quick Take — Titan Company**
- CMP ₹4,372 · P/E 80.0x · ROE 37.7% · ROCE 20.5% (Source: Screener)
- Flagged as "Expensive" on valuation, "Strong" on fundamental quality
- Skill correctly flagged unavailable sector-P/E data with 🚩 instead of guessing

**Compare — TCS vs Infosys**
- Side-by-side table: CMP, Market Cap, P/E, historical ROE
- No winner declared, per skill rules — just "Where A Leads" / "Where B Leads"

## Key Finding
Live financial data across sources (Screener, Tijori, Equitymaster, TipRanks) 
disagreed meaningfully — ROE figures for the same company varied by 10+ 
percentage points depending on the article's age. This validated why the 
skill's **mandatory 2-source cross-check rule** matters: without it, the report 
would silently present stale numbers as current fact.

## Key Learning
A skill is only as reliable as its guardrails. The most valuable lines in this 
skill weren't the output formatting — they were the constraints: "never 
fabricate data," "flag if unavailable," "cite every figure," "no buy/sell 
calls." These turn a plausible-sounding financial summary into something 
closer to a defensible research aid. Once saved, the skill is reusable — 
future stock queries pull the same rigor without re-typing the whole prompt.

## Screenshots
<img width="533" height="636" alt="image" src="https://github.com/user-attachments/assets/74657a23-1951-40c8-994f-de3e198b49e9" />

<img width="575" height="592" alt="image" src="https://github.com/user-attachments/assets/83001723-d4c9-444c-8795-57e93baf2db2" />


#60DayClaudeChallenge
