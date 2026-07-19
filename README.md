# Covered-call rolling on real open interest

Own shares, sell the monthly call where open interest is highest (including
in-the-money magnets), and roll **up-and-out** for a net credit after run-ups
(never roll the strike down). ITM short calls buffer downside; upside remains capped.

Sixteen large caps, 2020–2025, real OCC open interest (ThetaData).

Live: https://elliottshort.github.io/ten-percent-week/
