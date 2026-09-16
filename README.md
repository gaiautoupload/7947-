# 7947 PieceMakers broker-flow radar

Static GitHub Pages dashboard for Taiwan emerging-market stock 7947. The site reads `data/snapshot.json` and requires no backend or database.

The matching tracker lives in `../7947_strategy`. It starts history on the stock's first trading date, 2026-09-16, rebuilds broker inventory and estimated cost from TPEx EMdss004 price-level records, and updates this repository's snapshot.

The 7947 playbook is intentionally in sample-building mode for the first five valid trading days. A first-day order is not treated as a confirmed controlling broker. Impact ranking only becomes active after enough next-day observations exist.

To publish later, create a GitHub repository for this directory, push the `main` branch, and enable GitHub Pages from the repository root.
