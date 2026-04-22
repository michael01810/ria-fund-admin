RIA & Fund Admin Analytics

Using SEC adviser registration and Form ADV to analyze growth and quality of RIAs and fund adminstration players

## Features

- RIA (daily frequency)
  - advisor count
  - advisor growth
  - advisor tenure
  - advisor attrition
  - advisor quality (customized)
  - AUM growth (frequency as reported)
  - AUM / advisor

- Fund Admin (frequency as reported)
  - fund admin player by customer count, AUM, geography, fund type etc.
  - customer switching
  - fund admin customer churn / expansion
 
  **Point your LLM at the data to answer questions like**:
  - which fund admin firms have been expanding market share among real estate funds over the past 2 years (show relevant raw data)
  - which fund admin firms are most exposed to private credit fund withdrawls seen in the news in 2026
  - % churn by AUM & fund count for top 20 fund admin firms by AUM serviced
  - After LPL announced its acquisition of Commonwealth, how many advisors left and where to
  - Assuming market returns, which RIAs in the $5 - $50 billion AUM range have seen the highest growth in AUM / advisor

## RIA Example
<img width="1855" height="705" alt="RIA example" src="https://github.com/user-attachments/assets/18b76366-50fd-4ad5-8a8b-5704e19afb3c" />

- Advisor growth from April 2025 to April 2026; AUM reported in March / April 2026 are generally year-end 2025 figures
- Join = lateral hires from other RIAs. Does not include new grad representatives which drags down YOE (years of experience) metric 

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
- fund_admin_output_firm.csv (firm-level -> GGV CAPITAL LLC)
- fund_admin_output_fund.csv (fund-level -> GGV CAPITAL VIII L.P.)
- Firm level history from 2000; fund level history from 2011

```

## Notes

Contact michaelsong01810@gmail.com for code and data access

