# Battery Optimisation Case (2018–2020)

This repository contains an optimisation model to determine the optimal charge/discharge schedule of a battery across three electricity markets, maximising arbitrage profit over the 2018–2020 period.

---

## Objective
Maximise battery trading profit while operating as a **price-taker** across three electricity markets:
- **Market 1**: half-hourly prices
- **Market 2**: half-hourly prices
- **Market 3**: daily price with **constant power commitment throughout the day**

---

## Approach overview
- The model performs **energy arbitrage** by charging when prices are low and discharging when prices are high.
- Decisions are:
  - **Half-hourly** for Markets 1 and 2
  - **Daily constant-power** for Market 3
- The model includes:
  - battery **power** and **energy** limits,
  - **state-of-charge (SoC)** dynamics,
  - charging/discharging **efficiency losses**,
  - **mutual exclusivity** between charging and discharging (MILP).

---
