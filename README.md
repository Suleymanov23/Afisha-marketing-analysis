# Afisha Marketing Analysis

Analysis of user behavior and marketing spend for Yandex.Afisha, an events and tickets platform. The goal: understand how people use the product, when they convert to buyers, how much revenue each customer brings, and which marketing sources are actually worth the money.

## What's inside

- `afisha_marketing_analysis.ipynb` - the full analysis, step by step
- `visits_log_us.csv` - session logs
- `orders_log_us.csv` - purchase logs
- `costs_us.csv` - daily marketing spend per source

## What I looked at

**Product usage**
- DAU / WAU / MAU and sticky factor
- Session count and session length
- Retention by acquisition cohort
- Device split (desktop vs mobile) and weekly traffic pattern

**Sales**
- Time from first visit to first purchase
- Orders per month and average order value
- LTV per user by cohort

**Marketing**
- Total and per-source ad spend
- CAC (customer acquisition cost) per source
- ROMI (return on marketing investment) per source and per cohort over time

## Key findings

- Only **4 out of 8** paid sources have a positive ROMI. Source 1 performs best (+49%); source 3 is the worst (-61%) despite having one of the largest budgets.
- The cheapest source to acquire users (source 10, $4.38 CAC) is still **not profitable** (-24% ROMI) - low cost doesn't mean good traffic.
- Overall, the company spent about **$329K** and earned back about **$252K** - marketing has not fully paid for itself yet, and newer cohorts are trending worse than older ones.
- **72%** of buyers purchase on the same day as their first visit - this is a fast-decision product, not one that needs long nurturing campaigns.
- Desktop drives **73%** of sessions and the large majority of revenue; weekday traffic is consistently higher than weekend traffic.

Full explanation and numbers are in the notebook, with notes before and after every step describing what was done and why.

## Tools used

Python, pandas, numpy, matplotlib, seaborn, scipy
