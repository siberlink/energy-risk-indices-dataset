# Daily Index Schema

Each CSV file contains daily index observations for one EnergyRiskIQ risk index.

## Files

- `data/geri_daily.csv`
- `data/eeri_daily.csv`
- `data/egsi_daily.csv`

## Columns

| Column | Type | Description |
|---|---|---|
| `date` | date | Observation date in `YYYY-MM-DD` format |
| `index_code` | string | Index identifier: `GERI`, `EERI`, or `EGSI` |
| `index_name` | string | Full name of the index |
| `value` | number | Index value on a 0–100 scale |
| `risk_band` | string | Risk level classification |
| `change_1d` | number | Daily change versus previous observation |
| `notes` | string | Optional short context note |

## Risk Scale

| Value Range | Risk Band |
|---|---|
| 0–20 | Low |
| 21–40 | Elevated |
| 41–60 | High |
| 61–80 | Severe |
| 81–100 | Critical |

## Date Format

All dates use ISO format:

```text
YYYY-MM-DD
