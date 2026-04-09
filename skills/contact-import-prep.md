# Skill: Contact Import Preparation

## Purpose
Takes a raw contact CSV/XLSX and prepares it for clean import into HubSpot — deduplication, validation, territory filtering, exclusion checking, and property mapping.

## When to Use
- Aalia shares a new contact list (trade show, purchased list, referral, Salesforce export)
- ZoomInfo search results need to be imported
- Bulk contact updates from any external source

## Process

### Step 1: Initial Assessment
- How many contacts in the file?
- What columns/fields are present?
- What's the data quality at a glance? (missing emails, blank fields, formatting issues)

### Step 2: Data Cleaning
- Standardize column names to match HubSpot properties
- Clean email formats (remove spaces, fix obvious typos like .con → .com)
- Standardize city/state names
- Remove obviously invalid entries (test@test.com, no-email, blank rows)
- Split combined fields if needed (full name → first name + last name)

### Step 3: Deduplication (Internal)
- Remove duplicates within the import file itself
- Match by email (exact), then by practice name + city (fuzzy)

### Step 4: Deduplication (Against HubSpot)
- Check every contact against existing HubSpot database
- Match by email (primary), then practice name + city (secondary)
- Flag existing contacts: should they be updated or skipped?
- New contacts only proceed to import

### Step 5: Territory Filter
- Check every contact's city/state against approved territory
- Oklahoma: all pass
- Texas: only DFW metro, Midland, Odessa, and assigned regions
- Everything else: removed with explanation

### Step 6: Exclusion Filter
- Cross-reference against Salesforce exclusion list
- Match by practice name (primary) and email domain (secondary)
- Any match: removed from import, flagged in report

### Step 7: Property Mapping
Map import columns to HubSpot properties:
| Import Column | HubSpot Property |
|--------------|-----------------|
| Email | email |
| First Name | firstname |
| Last Name | lastname |
| Practice Name | company |
| City | city |
| State | state |
| Phone | phone |
| Specialty | specialty (custom) |
| Notes | notes |

Set defaults for new contacts:
- `lifecyclestage` = lead
- `btl_lead_priority` = Cold (unless specified)
- `hs_lead_status` = NEW

### Step 8: Final Report
```
---
IMPORT PREPARATION REPORT
Source: [file name]
Date: [date]
---

## Summary
- Raw contacts in file: [#]
- Removed (invalid/incomplete): [#]
- Removed (internal duplicates): [#]
- Removed (already in HubSpot): [#]
- Removed (outside territory): [#]
- Removed (Salesforce exclusion): [#]
- READY TO IMPORT: [#]

## Breakdown of Import-Ready Contacts
- By state: [OK: #, TX: #]
- By city: [top cities]
- By specialty: [if available]

## Flagged for Review
- [contacts that need manual decision]

## Next Steps
- Approve import → will add [#] contacts to HubSpot
- Recommend assigning to Aalia (Owner ID 88459377)
- Suggest initial outreach priority: [recommendation]
```

### Step 9: CEO Approval
Present the report. Aalia approves before any contacts are imported.

## Quality Checks
- [ ] No duplicate imports (checked against HubSpot)
- [ ] Territory filter applied
- [ ] Exclusion list checked
- [ ] Property mapping is correct
- [ ] Invalid emails removed
- [ ] Report includes clear summary for approval decision
