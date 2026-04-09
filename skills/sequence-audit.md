# Skill: Sequence Audit

## Purpose
Analyzes HubSpot sequence performance, identifies issues, and recommends optimizations. This is the diagnostic tool for understanding what's working and what's broken in your outreach sequences.

## When to Use
- Weekly sequence performance check
- When bounce rate exceeds 5% on any sequence
- Before launching a new sequence (learn from what worked)
- When engagement drops unexpectedly
- When Aalia asks "how are our sequences doing?"

## Audit Dimensions

### Deliverability Health
- Bounce rate per sequence (threshold: >5% = problem)
- Bounce rate per email step (is one email bouncing more than others?)
- Domain-level blocks (are certain email domains rejecting us?)
- Spam complaint signals (if available)

### Engagement Analysis
- Open rate per email (benchmark: 20-25% for cold, 30-40% for warm)
- Click rate per email (benchmark: 3-5% for cold, 8-12% for warm)
- Reply rate per email (benchmark: 2-4% for cold, 5-8% for warm)
- Engagement by email position (which step in the sequence performs best?)
- Drop-off analysis (where do people stop engaging?)

### Task & Signal Analysis
- Tasks created per sequence (watch for junk task inflation)
- "2 opens or 1 click" threshold accuracy — how many are bot opens vs. real?
- Reply sentiment breakdown: positive, neutral, negative, opt-out
- Meeting requests vs. declines vs. questions

### Sequence Completion
- How many contacts complete all steps with no engagement (wasted outreach)
- How many complete with engagement but no conversion (need different approach)
- How many drop out mid-sequence and why

### Subject Line Performance
- Rank subject lines by open rate
- Identify patterns in top performers
- Flag underperformers for A/B testing

## Output Format
```
---
SEQUENCE AUDIT REPORT
Period: [date range]
Sequences Analyzed: [#]
---

## Health Score: [Green/Yellow/Red]

## Top Findings
1. [Most important insight]
2. [Second insight]
3. [Third insight]

## Per-Sequence Breakdown
[Table: sequence name, enrolled, completed, bounced, open rate, click rate, reply rate, health score]

## Recommendations
- [Specific, actionable improvement with expected impact]

## Alerts
- [Any urgent issues requiring immediate attention]
```

## Quality Checks
- [ ] Metrics are calculated correctly (not double-counting)
- [ ] Benchmarks are appropriate for the outreach type (cold vs. warm)
- [ ] Bot open inflation is accounted for in engagement metrics
- [ ] Recommendations are specific and actionable (not generic)
