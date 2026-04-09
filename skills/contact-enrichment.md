# Skill: Contact Enrichment

## Purpose
Enriches existing HubSpot contacts with additional data points to improve segmentation, personalization, and outreach targeting.

## When to Use
- Before launching a new outreach campaign
- When contact records are missing key fields (specialty, phone, decision maker name)
- Bulk enrichment of imported contact lists
- Preparing event invitation lists

## Inputs Required
- **Contact list or criteria**: Which contacts to enrich (e.g., "all contacts in Tulsa with no specialty set")
- **Fields to enrich**: Which data points are needed
- **Priority**: Which contacts matter most (Hot > Warm > Cold)

## Enrichment Fields
| Field | Source | Priority |
|-------|--------|----------|
| Practice specialty | ZoomInfo / Web search | High |
| Decision maker name + title | ZoomInfo | High |
| Direct phone number | ZoomInfo | Medium |
| Practice website | Web search | Medium |
| Number of locations | Web search | Low |
| Current aesthetic devices | Web search / competitor intel | Medium |
| Social media profiles | Web search | Low |
| Product interest | HubSpot activity data | High |

## Process
1. Export or query the target contact list from HubSpot
2. For each contact, check which fields are missing
3. Use ZoomInfo enrichment tools to fill gaps
4. Cross-reference with web search for practice-specific details
5. Flag any contacts that appear inactive or invalid
6. Produce enrichment report with recommendations

## Output Format
```
---
ENRICHMENT REPORT
Contacts processed: [#]
Fields updated: [#]
Date: [date]
---

## Summary
- Contacts enriched: [#]
- Contacts with no data found: [#]
- Invalid/inactive contacts flagged: [#]

## Key Findings
[Notable patterns — e.g., "42% of unenriched contacts are dental practices"]

## Recommended Actions
- [Action items based on enrichment results]

## Detailed Results
[Table or list of enriched contacts with before/after data]
```

## HubSpot Custom Properties to Update
- `specialty` — Practice specialty
- `outreach_type` — Event / Product / Both
- `product_interest` — Multi-checkbox (Emvital, Emsella, Emsculpt NEO, Exion, Emface, Emtone, Starformer)
- `target_event` — Tulsa / Dallas
- `btl_lead_priority` — Hot / Warm / Cold

## Quality Checks
- [ ] No duplicate enrichment (check if field already has data)
- [ ] Data sources are reliable
- [ ] Invalid contacts flagged, not silently skipped
- [ ] HubSpot property names match exactly
- [ ] Enrichment report includes actionable next steps
