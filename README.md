# Kalshi Subaccounts — settled results per trader

Static dashboard of settled P&L per Kalshi subaccount (attributed by fill-cost
share, since subaccount is recorded only on fills). All-time / Last 30 / Last 7 /
Yesterday windows.

Live page: https://gehrenberg823.github.io/kalshi-subaccounts/

Snapshot only — regenerated and pushed manually (the data-refresh tooling is
kept private).

## Updating the shared page
    cd ~/KalshiSubaccounts
    python3 refresh.py            # regenerate subaccounts.html (needs prod CH creds)
    cp subaccounts.html docs/index.html
    git commit -am "refresh" && git push
