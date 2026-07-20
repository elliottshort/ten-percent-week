# Covered-call rolling on real open interest

Own shares, sell the monthly call where open interest is highest (including
in-the-money magnets), and roll **up-and-out** for a net credit after run-ups
(never roll the strike down). ITM short calls buffer downside; upside remains capped.

Sixteen large caps, 2020–2025, real OCC open interest (ThetaData).

**Latest re-run (no roll-down):** median strategy CAGR **+12.6%** vs B&H **+18.6%**;
NVDA **+37.1%** vs **+77.4%**; **~37%** ITM-at-write; **141** forced assignments;
**0** roll-downs.

Live: https://elliottshort.github.io/ten-percent-week/
