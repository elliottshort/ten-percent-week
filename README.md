# Trend-gated selective harvest vs buy-and-hold

Walk-forward covered-call overwrite on **32** large caps (2020–2025), compared to
fair continuous buy-and-hold with daily dividend reinvestment.

**Policy (TGSH, IS-frozen on core 16):** write only when name 63d return ≤ −10% and the
equal-weight market 63d ≤ 0; coverage scales with crash depth; OTM band;
jump-to-expiry; ITM close-hold when the gate clears. Thresholds are **not** re-tuned
on holdouts or OOS.

**Expanded universe (N=32, need ≥18 beating B&H):**
- Full median TGSH **+14.0%** vs fair B&H **+14.4%**
- Equal-weight basket TGSH **+23.9%** vs B&H **+23.5%**
- Breadth **16 of 32** (edge verdict: `edge_fails_gates`)
- OOS median **+21.4%** vs **+23.6%**; **15 of 32** beat

**Core 16 (selection set):** 11/16 beat hold
(med edge +0.4%).
**Holdout 16 (stress only):** 5/16 beat hold
(med edge −0.2%).

Source study & engine: [buywrite-backtest](https://github.com/elliottshort/buywrite-backtest).

Live: https://elliottshort.github.io/ten-percent-week/
