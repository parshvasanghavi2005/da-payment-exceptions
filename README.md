# Payment Exception Analysis

**Type:** Data analysis portfolio project. **Domain:** FinTech and finance operations. **Data:** 80 deterministic, synthetic payment cases.

Run `python3 analyze.py` from this repository root. The script regenerates `synthetic_payments.csv` and `report.md` with no external packages.

## Questions answered

1. What share of orders needs investigation?
2. Which exception reason accounts for the largest amount to investigate?
3. Which merchants have the largest exception totals?
4. How many cases are aged 0–2, 3–7, and 8+ days?

## Method

The Python script uses a fixed random seed so its 80 rows are reproducible. It groups exception records by reason and merchant, sums integer paise, computes an exception rate, and segments case age. The output is a readable Markdown report for an operations lead.

**Important:** The amount to investigate is a synthetic triage metric, not a booked loss, fraud score, or real financial exposure. Prioritize cases only after checking source transaction evidence. No causal inference or business impact claim is made from generated data.
