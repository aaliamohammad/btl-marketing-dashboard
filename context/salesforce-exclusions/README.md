# Salesforce Exclusion List

## What Goes Here
Drop your Salesforce export here — a CSV or XLSX file containing practices that already have BTL devices and/or have an assigned PSM.

## What I Need in the Export
At minimum, these columns:
- **Practice/Account Name** (required)
- **City, State** (required)
- **Contact Email** or **Email Domain** (helpful for matching)
- **PSM Name** (helpful to know whose territory it is)
- **Devices Owned** (helpful for context)

## How It's Used
Before any outreach campaign, every contact is cross-referenced against this list. If their practice appears here, they are excluded from cold outreach.

## How to Update
Just drop a new export here. The most recent file will be used. Name it with the date so we know how fresh it is (e.g., `salesforce_exclusions_2026-04-09.csv`).
