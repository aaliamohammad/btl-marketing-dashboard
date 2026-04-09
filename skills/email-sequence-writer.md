# Skill: Email Sequence Writer

## Purpose
Creates multi-step email sequences for HubSpot outreach campaigns. Each sequence follows BTL's communication style and is designed for automated delivery with smart send windows.

## When to Use
- Building new outreach sequences (cold, warm, or re-engagement)
- Creating product-specific email series
- Developing nurture sequences for different practice types

## Inputs Required
- **Sequence goal**: What action should the recipient take? (register for event, book a meeting, request a demo)
- **Target audience**: Practice type (aesthetics, wellness, derm, OB/GYN, dental, med spa)
- **Number of emails**: Typically 3-6 emails
- **Cadence**: Days between each email (e.g., Day 1, Day 3, Day 7)
- **Product focus** (optional): Which BTL devices to highlight
- **Event details** (optional): If event-driven, include event name, dates, location

## Output Format
For each email in the sequence, produce:
```
---
Email [#] of [total] | Send: Day [X]
Subject: [subject line]
---

[Email body]

[Signature block]
---
Internal notes:
- Goal of this email: [what this touchpoint achieves]
- If no response: [what the next email addresses]
```

## Style Rules (from CLAUDE.md)
- Warm, low-pressure, peer-level tone
- NO em dashes in body copy
- Short paragraphs (2-3 sentences max)
- Reference prior touchpoints for continuity between emails
- Each email should feel like a natural progression, not a repeat
- General office emails: open with "Hi there"
- Named contacts: use first name only
- Always include both event dates when applicable (Tulsa + Dallas)
- Leave format options open (in-person lunch meeting OR virtual)
- Signature: Aalia Mohammad | Practice Success Manager | [phone] | [email]

## Sequence Architecture
- **Email 1**: Introduction + value prop + soft CTA
- **Email 2**: Social proof or case study + specific benefit for their practice type
- **Email 3**: Direct ask with urgency element (limited spots, date approaching)
- **Email 4** (if needed): Different angle or new information
- **Email 5** (if needed): Final touch — low-pressure, keep the door open
- **Breakup email** (last): Acknowledge silence, leave door open, no guilt

## Quality Checks
- [ ] No em dashes anywhere
- [ ] Each email has a distinct purpose (not repetitive)
- [ ] Subject lines are under 50 characters
- [ ] CTAs are clear but not pushy
- [ ] Practice-type specific language is accurate
- [ ] Signature block is consistent
- [ ] Reply subject lines maintain threading with "Re:" prefix
