# redgrave-platform

AFC Redgrave data platform — Data Engineering & Cloud Infrastructure labs (Albert School).

| Folder | Lab | What it does |
|---|---|---|
| `redgrave_dbt/` | RED-202 · dbt inside Snowflake | Bronze → silver (3 views) → gold (3 tables), 18 tests, source freshness, deployed as a Snowflake `DBT PROJECT` scheduled by a task |

Expected result: `GOLD_REVENUE_BY_CHANNEL` totals **21,436 GBP**, `dbt build` → `PASS=25`.

No secret in this repository: `profiles.yml` contains no account, user, password or key (dbt runs inside Snowflake).
