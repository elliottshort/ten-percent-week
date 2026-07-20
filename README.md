# Multi-horizon regime machine vs buy-and-hold

Walk-forward covered-call overwrite on **16** large caps (2020-2025), compared to fair continuous buy-and-hold with daily dividend reinvestment.

**Policy (IS-frozen `mh_machine_0106`):** classify each decision day into crisis / runner / pullback / mkt_weak / name_weak / calm from name momentum (21d, 63d), SPY 63d, and VIX. Each state sets coverage, OTM band, and equity deploy. No per-symbol parameters.

**Full sample:** median machine **+16.6%** vs B&H **+17.1%**; basket **+28.2%** vs **+26.8%**; **10 of 16** beat hold.

**OOS (2023-end):** median **+29.0%** vs **+29.1%**; basket **+40.8%** vs **+40.4%**; **10 of 16** beat hold.

OOS edge is thin. Thresholds were not re-tuned after the OOS look.

Source: [buywrite-backtest](https://github.com/elliottshort/buywrite-backtest).

Live: https://elliottshort.github.io/ten-percent-week/
