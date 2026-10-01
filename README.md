# CanPay Open Data — Canadian Take-Home Pay 2026

Open dataset of **net take-home pay, income tax, CPP/CPP2 and EI by province and income level** for the **2026** tax year, computed from the transparent rules engine behind [CanPay Insights](https://canpayinsights.ca) — a free Canadian take-home-pay calculator.

**Version 2026-09-15** (mirrors https://canpayinsights.ca/data; the site is the source of truth). **455 rows** — 13 provinces & territories × 35 income levels ($30,000–$200,000).

## Files
- [`canpay-take-home-2026.csv`](canpay-take-home-2026.csv) — 455 rows, 14 columns
- [`canpay-take-home-2026.json`](canpay-take-home-2026.json) — same data, JSON
- Always-current copies: https://canpayinsights.ca/data

## Columns
`year, province_slug, province, gross, net_annual, net_monthly, net_biweekly, federal_tax, provincial_tax, cpp_qpp_qpip, ei, total_deductions, average_tax_rate_pct, total_deduction_rate_pct`

## Sample — take-home on an $80,000 salary (2026)
| Province | Net (annual) |
|---|---|
| British Columbia | $61,157 |
| Ontario | $60,303 |
| Alberta | $60,698 |
| Quebec | $57,012 |

## Methodology
Published 2026 rates from the CRA, Revenu Québec, and each province/territory:
- Federal income tax (lowest bracket cut to 14% for 2026) + each province/territory's brackets
- CPP 5.95% to the YMPE (~$74,600) and CPP2 (+4%) to the YAMPE (~$85,000); QPP/QPIP for Quebec
- EI 1.63% to the maximum insurable earnings ($68,900); Quebec uses 1.30%
- Basic personal amount only (no other credits) — a clean, comparable baseline

Estimates for general information, not tax advice. Verify current-year figures with the CRA.

## License & citation
Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Free to share and adapt, including commercially, with attribution:

> CanPay Insights, *Canadian Take-Home Pay & Payroll Deductions 2026* (open dataset). https://canpayinsights.ca

## About
Built by **CanPay Insights** — a free, independent Canadian take-home-pay calculator (every province, CPP/CPP2, EI, EN/FR/中文, no signup). https://canpayinsights.ca
