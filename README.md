# 個股主力雷達

Static GitHub Pages dashboard for Taiwan emerging-market stocks 7947, 7949, 7950, 6610, 7951 and 6660. Each stock page reads its own `stocks/<stock_id>/data/snapshot.json` and requires no backend or database.

The matching tracker lives in `../7947_strategy`. It rebuilds broker inventory and estimated cost from TPEx EMdss004 price-level records and updates every configured stock snapshot.

Newly registered stocks, including 7951 and 6660 from 2026-10-06, remain in sample-building mode for their first five valid trading days. A first-day order is not treated as a confirmed controlling broker. Impact ranking only becomes active after enough next-day observations exist.

To publish later, create a GitHub repository for this directory, push the `main` branch, and enable GitHub Pages from the repository root.
