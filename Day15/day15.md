# Day 15 — Vedic Astrology & Life Analysis Prompt

## Task
Test a detailed, structured "expert Vedic astrologer" system prompt (Parashara, 
Jaimini, Nakshatra, Vimshottari Dasha, Transit Analysis) with Claude, following 
the standard intake → report → forecast → remedies pipeline.

## What Happened
Instead of generating placements and predictions from a birth date/time, Claude 
flagged a limitation upfront: accurate Vedic astrology requires real ephemeris 
calculations (planetary positions, ayanamsa correction, house systems, dasha 
math) that an LLM can't reliably compute from memory. Fabricated placements 
would look authoritative but be wrong.

Claude offered two paths:
1. Interpret the *framework* and explain methodology without real data
2. Take actual chart output from ephemeris software (AstroSage, Jagannatha 
   Hora) and interpret *that* using classical principles

## Key Learning
A well-structured prompt with clear sections, tables, and output rules doesn't 
guarantee reliable output if the underlying task needs deterministic computation 
the model can't do — this is a good stress test for **prompting vs. capability 
boundaries**. Elaborate prompt engineering can't substitute for a tool that does 
actual astronomical calculation. The right move is a model that names the 
limitation rather than confidently hallucinating planetary degrees.

## Takeaway for Prompt Design
For domains involving precise computation (astrology, astronomy, financial 
modeling with real market data, legal citations), pair the LLM with a 
calculation/data tool rather than asking it to "reason" the numbers from 
scratch. The LLM's job is structuring and interpreting — not computing.



#60DayClaudeChallenge
