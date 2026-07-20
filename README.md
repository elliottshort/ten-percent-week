# Trend-gated selective harvest vs buy-and-hold

Walk-forward covered-call overwrite on 16 large caps (2020–2025), compared to
fair continuous buy-and-hold with daily dividend reinvestment.

**Policy (TGSH, IS-frozen):** write only when name 63d return ≤ −10% and the
equal-weight market 63d ≤ 0; coverage scales with crash depth; OTM band;
jump-to-expiry; ITM close-hold when the gate clears.

**Full-sample headlines:** median TGSH CAGR **+17.6%** vs fair buy-and-hold
**+17.1%** (always-write baseline **+15.2%**); **11 of 16** names beat hold;
equal-weight basket TGSH **+27.9%** vs B&H **+26.9%**. OOS (2023–end, fresh
$100k): median **+29.9%** vs **+29.2%**; **10 of 16** beat.

Source study & engine: [buywrite-backtest](https://github.com/elliottshort/buywrite-backtest).

Live: https://elliottshort.github.io/ten-percent-week/
