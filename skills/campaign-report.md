# Skill: Campaign Report

## Purpose
Generates comprehensive campaign performance reports from HubSpot data, email metrics, and event registration tracking.

## When to Use
- Weekly or monthly campaign performance reviews
- Post-event ROI reporting
- Sequence performance analysis
- Preparing updates for Chad Coccaro (Area Sales Director) or leadership

## Inputs Required
- **Report type**: Weekly snapshot, monthly deep-dive, post-event, or sequence performance
- **Time period**: Date range for the report
- **Campaign/sequence name(s)**: Which campaigns to analyze
- **Comparison period** (optional): For trend analysis

## Report Sections

### Executive Summary
- 3-5 bullet overview of key metrics and takeaways
- Red/yellow/green status indicators

### Email Performance
- Emails sent, delivered, opened, clicked, replied
- Open rate and click rate (with benchmarks)
- Top performing subject lines
- Reply analysis (positive, negative, opt-out)

### Sequence Performance
- Contacts enrolled per sequence
- Completion rate (how many made it through all steps)
- Drop-off points (which email loses the most people)
- Task creation volume (and junk task identification)

### Event Registration (if applicable)
- Registrations by source (which sequence/email drove them)
- Registration rate by practice type
- Geographic distribution
- Pending vs. confirmed registrations

### Pipeline Impact
- Meetings booked from outreach
- New opportunities created
- Contacts moved from Cold → Warm → Hot
- Revenue attribution (if available)

### Recommendations
- What's working and should be scaled
- What's underperforming and needs adjustment
- Specific next steps with owners

## Output Format
Produce as both:
1. **Markdown report** (for internal review)
2. **Excel dashboard** (for data visualization) — use the xlsx skill

## Data Sources
- HubSpot CRM (contacts, sequences, workflows)
- HubSpot email analytics
- Event registration data
- Manual tracking data (if provided)

## Quality Checks
- [ ] All metrics are calculated correctly
- [ ] Comparison to previous period included where relevant
- [ ] Recommendations are specific and actionable
- [ ] No vanity metrics without context
- [ ] Report is formatted for the intended audience
