# Aurora_technicalquestion
# Battery Optimisation Case (2018–2020)

This repository contains an optimisation model to determine the optimal charge/discharge schedule of a battery across three electricity markets, maximising arbitrage profit over the 2018–2020 period.

## Approach overview
- The battery is modelled as a **price-taker**.
- **Half-hourly** decisions are taken for Markets 1 and 2.
- A **daily** decision is taken for Market 3 (constant power throughout the day).
- The model includes:
  - power and energy (SoC) limits,
  - state-of-charge (SoC) transition dynamics,
  - charging/discharging efficiencies,
  - a mutual exclusivity constraint preventing simultaneous charge and discharge (MILP).

## Requirements
- Python 3.9+ (recommended)
- HiGHS solver (via `highspy`)

## Installation
```bash
pip install -r requirements.txt
