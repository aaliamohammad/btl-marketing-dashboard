# Skill: HubSpot Data Cleanup

## Purpose
Performs bulk data hygiene operations on the HubSpot contact database — deduplication, missing field identification, bounce cleanup, stale record detection, and property standardization.

## When to Use
- Before launching any new outreach campaign (clean data = better deliverability)
- After importing a new contact list
- When bounce rates exceed 5% on any sequence
- Monthly data health audit
- When Aalia asks "how clean is our data?"

## Cleanup Operations

### Deduplication
- Match criteria (in priority order):
  1. Exact email match (definite duplicate)
  2. Same practice name + same city (likely duplicate)
  3. Same last name + same practice name (possible duplicate — flag for review)
- Action: Merge duplicates, keeping the record with more data populated
- Always present merge candidates to Aalia before executing

### Bounce Cleanup
- Pull all contacts with "hard bounce" email status
- Categorize: invalid email, domain doesn't exist, mailbox full (soft), blocked by server
- Hard bounces: flag for enrichment (find updated email via ZoomInfo)
- Soft bounces: flag for retry in 48-72 hours
- Chronic bounces (bounced 2+ times): recommend removal or archival

### Missing Data Identification
- Scan for contacts missing critical fields:
  - Email (can't do anything without it)
  - City/State (can't territory-filter without it)
  - Specialty (needed for practice-type segmentation)
  - BTL Lead Priority (needed for scoring)
  - Outreach Type (needed for campaign targeting)
- Report: count per missing field, percentage of database, recommendations

### Stale Record Detection
- Contacts with no activity in 6+ months (no opens, clicks, replies, form submissions)
- Contacts enrolled in completed sequences with zero engagement
- Contacts with outdated information (e.g., old email domains)
- Recommendation: re-enrich, archive, or flag for manual review

### Property Standardization
- Check for inconsistent values (e.g., "aesthetics" vs "Aesthetics" vs "aesthetic")
- Validate dropdown/multi-select values match HubSpot property options
- Flag free-text fields that should be standardized

## Output Format
```
---
DATA CLEANUP REPORT
Date: [date]
Contacts Scanned: [#]
---

## Summary
- Duplicates found: [#]
- Hard bounces: [#]
- Missing critical fields: [#]
- Stale records: [#]
- Property issues: [#]

## Priority Actions
1. [Highest impact action]
2. [Second priority]
3. [...]

## Detailed Findings
[Section per cleanup category with specifics]
```

## Quality Checks
- [ ] Never delete contacts without Aalia's approval
- [ ] Always present merge candidates before executing
- [ ] Preserve the most complete record when merging
- [ ] Flag uncertain matches for manual review
- [ ] Track cleanup actions for audit trail
