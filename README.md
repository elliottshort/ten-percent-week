# Covered-call rolling on real open interest

A six-year backtest of covered-call premium harvesting with rolling:

1. Own the shares
2. Sell the monthly call where open interest is highest
3. At expiry, keep dead premium or roll up-and-out for a net credit
4. Reinvest premium into more lots

Sixteen large caps, 2020–2025, real OCC open interest (ThetaData) for every strike pick.

Live page: https://elliottshort.github.io/ten-percent-week/

Engine and drivers live in the companion `buywrite-backtest` repo (`wheel_bt/harvest.py`, `run_harvest.py`).
