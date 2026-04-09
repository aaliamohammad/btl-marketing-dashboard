# Skill: Post-Event Follow-Up

## Purpose
Creates segmented post-event follow-up sequences based on attendee engagement level and expressed interest.

## When to Use
- After any BTL event or symposium
- Following a demo day or lunch-and-learn
- After trade show or conference interactions

## Inputs Required
- **Event name and date**: Which event just happened
- **Attendee segments**: 
  - Hot: Expressed strong interest, asked about pricing/ordering
  - Warm: Attended, engaged, but no commitment
  - Attended but passive: Showed up, minimal engagement
  - No-show: Registered but didn't attend
- **Products discussed** (if known): Which BTL devices generated interest
- **Key conversations** (if available): Notable interactions to reference

## Output Format
One follow-up sequence per segment:
```
---
SEGMENT: [Hot / Warm / Passive / No-Show]
---

Email 1 | Send: [timing post-event]
Subject: [subject]
[Body]

Email 2 | Send: [timing]
Subject: [subject]
[Body]

[Additional emails as needed per segment]
```

## Segment Strategy

### Hot Leads (2-3 emails, fast cadence)
- Email 1 (next day): Personal thank you, reference specific conversation, propose next step (demo, pricing call)
- Email 2 (3 days later): Share relevant case study or ROI data
- Email 3 (1 week): Gentle close or meeting proposal

### Warm Leads (3-4 emails, moderate cadence)
- Email 1 (next day): Thank you, event recap highlights
- Email 2 (4 days): Share content related to their practice type
- Email 3 (1 week): Offer personalized demo or lunch meeting
- Email 4 (2 weeks): Low-pressure check-in

### Passive Attendees (2-3 emails, slower cadence)
- Email 1 (next day): General thank you, one key takeaway
- Email 2 (1 week): Share a compelling piece of content
- Email 3 (2 weeks): Offer intro meeting, keep it casual

### No-Shows (2 emails)
- Email 1 (next day): "We missed you" — share event highlights, no guilt
- Email 2 (1 week): Offer alternative (virtual demo, next event mention like Dallas)

## Style Rules
- Reference specific event moments (not generic "great event!")
- Hot lead emails should feel like continuing a conversation
- No-show emails should be guilt-free
- Always mention the next upcoming event as an alternative
- NO em dashes
- Short paragraphs

## Quality Checks
- [ ] Each segment has appropriate urgency level
- [ ] Hot leads get fastest follow-up
- [ ] No-show emails are gracious, not guilt-tripping
- [ ] Next event mentioned where appropriate
- [ ] No em dashes
- [ ] Practice-specific personalization where possible
