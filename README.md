# Adviser Info (RIA & Fund Admin)

Using SEC adviser registration and Form ADV to analyze growth and quality of RIAs and fund adminstration players

## Features

- RIA (daily frequency)
  - advisor count
  - advisor growth
  - advisor tenure
  - advisor attrition
  - advisor quality (customized)
  - AUM / growth (frequency as reported)

- Fund Admin (frequency as reported)
  - fund admin player by customer count, AUM, geography etc.
  - customer switching 

## RIA Example
<img width="1855" height="705" alt="RIA example" src="https://github.com/user-attachments/assets/18b76366-50fd-4ad5-8a8b-5704e19afb3c" />

## Fund Admin Example
<img width="1756" height="643" alt="Fund admin example" src="https://github.com/user-attachments/assets/f131cd4c-5a66-4167-a9ac-d725caf2b785" />

## Setup

```bash
# 1. Clone the repo
git clone https://github.com/michael01810/ria-fund-admin.git
cd investment-adviser

# 2. RIA
run advisor_data_pull.py, fund_admin_data_pull.py, advisor_summary.py to get:
- advisor_raw_data.csv: full career history of each registered investment advisor representatives (person-level view)
- advisor_summary_output.xlsx: templated summary table showing grwoth and quality of each RIA (firm-level view)

# 3. Fund Admin
run fund_admin_data_pull.py to get:
- form_adv_output_firm.csv (firm-level -> GGV CAPITAL LLC)
- form_adv_output_fund.csv (fund-level -> GGV CAPITAL VIII L.P.)
- Firm level history from 2000; fund level history from 2011

```

## Notes


