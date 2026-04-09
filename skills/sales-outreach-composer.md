# Skill: Sales Outreach Composer

## Purpose
Creates personalized, multi-channel outreach plans for converting prospects into event attendees or product demo meetings. This is the tactical execution skill for the Sales Dev agent — it composes the actual messages and outreach sequences.

## When to Use
- Launching outreach to a new prospect list
- Creating personalized first-touch messages for high-value targets
- Building multi-channel sequences (email + SMS + call scripts)
- Re-engaging cold contacts in the HubSpot database

## Inputs Required
- **Prospect list or criteria**: Who are we reaching out to?
- **Outreach goal**: Event registration, demo meeting, intro call, or product interest
- **Channel(s)**: Email only, Email + SMS, Email + SMS + Call
- **Personalization data**: Practice name, specialty, location, any prior touchpoints
- **Urgency level**: Standard, time-sensitive (event approaching), or priority (hot lead)

## Multi-Channel Sequence Template
```
---
OUTREACH PLAN
Target: [prospect or segment]
Goal: [desired action]
Channels: [email / SMS / call]
Duration: [X days]
---

## Day 1: Email
Subject: [subject]
[Body]

## Day 2: SMS (if phone available)
[Short text message — under 160 characters]

## Day 3: Call Script
Opening: [what to say when they pick up]
Voicemail: [what to leave as a message]

## Day 5: Follow-up Email
Subject: Re: [original subject]
[Body]

## Day 8: Final Touch
[Channel and message based on engagement so far]
```

## SMS Guidelines
- Under 160 characters
- Casual but professional
- Include Aalia's name for recognition
- Clear CTA (reply YES, click link, call back)
- Note: Twilio A2P 10DLC registration pending — flag SMS as "ready when approved"

## Call Script Guidelines
- Opening: Introduce yourself and BTL, reference why you're calling
- If gatekeeper: Ask for the decision maker by name (if known from research)
- If voicemail: 30 seconds max, leave name + reason + callback number
- Always offer to send information via email as a follow-up

## Personalization Tiers
- **Tier 1 (High-value)**: Fully personalized — reference their practice, services, and specific BTL product fit
- **Tier 2 (Medium)**: Practice-type personalized — reference their specialty and relevant BTL products
- **Tier 3 (Bulk)**: Segment-level personalization — practice type + event/offer

## Quality Checks
- [ ] Each touchpoint has a clear purpose and builds on the last
- [ ] SMS messages are under 160 characters
- [ ] Call scripts sound natural, not robotic
- [ ] No em dashes in any written copy
- [ ] Personalization level matches the prospect value
- [ ] Multi-channel timing doesn't feel aggressive
- [ ] SMS flagged as pending if Twilio not yet active
