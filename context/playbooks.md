# BTL Marketing Team — Campaign Playbooks

These are the standard operating procedures for common tasks. When a task matches a playbook, the VP executes it without asking unnecessary questions. Only pause for CEO approval at the designated checkpoints.

---

## PLAYBOOK 1: Event Sequence Launch

**Trigger**: "Let's run a sequence for [event]" or "Set up [event] outreach"

### Auto-Known Context
- **Tulsa Event**: The Modern Medicine Symposium, April 24-26, Hyatt Regency Tulsa Downtown
- **Dallas Event**: June 5-7, Hotel ZaZa Dallas
- **Eye doctors** get "The Art of the Eyes" branding; all others get "The Modern Medicine Symposium"
- Signature: Aalia Mohammad | Practice Success Manager
- CC: labruzzojo@btlnet.com on prospect comms

### Execution Steps
1. **Intelligence pulls contacts:**
   - Filter by territory (OK + assigned TX regions)
   - Filter by proximity to event venue
   - Exclude Salesforce exclusion list matches
   - Exclude contacts currently in an active sequence
   - Exclude hard bounces and opt-outs
   - Segment by practice type (for branding: eye doctors separate)
   - Score by priority: Hot > Warm > Cold
   - Output: filtered contact list with count + breakdown

2. **Marketing creates event package:**
   - Event invite email copy (using event-invite-creator skill)
   - Landing page (if needed)
   - Social promotion posts (if requested)
   - All copy goes through confidentiality check (NO speaker/vendor names unless CEO approves)

3. **Sales Ops drafts the sequence:**
   - 4-5 email sequence using email-sequence-writer skill
   - Each email has a distinct angle (intro → value → urgency → different angle → breakup)
   - Cadence: Day 1, Day 3, Day 7, Day 12, Day 18 (adjustable)
   - Eye doctor segment gets separate sequence with Art of the Eyes branding
   - Both events mentioned where applicable

4. **VP assembles and presents to CEO:**
   - Contact list (count + practice type breakdown + territory breakdown)
   - Full sequence copy (all emails)
   - Enrollment plan (who gets enrolled, which sequence, timing)
   - Flag any edge cases

5. **CEO APPROVAL CHECKPOINT** ← Nothing moves past here without Aalia's sign-off

6. **Post-approval execution:**
   - Enroll contacts in HubSpot sequence
   - Set up monitoring for replies and engagement

---

## PLAYBOOK 2: Bounce Recovery & Enrichment

**Trigger**: "Who bounced?" or "Clean up the data" or proactively when bounce rate >5%

### Execution Steps
1. **Intelligence analyzes bounces:**
   - Pull bounce data from HubSpot sequences
   - Calculate bounce rate per sequence
   - Identify patterns (domain-level blocks, invalid emails, full mailboxes)
   - Categorize: hard bounce (invalid) vs. soft bounce (temporary)

2. **Intelligence runs enrichment:**
   - Hard bounces: ZoomInfo lookup for updated email addresses
   - If no ZoomInfo match: web search for practice website → find contact form or alternate email
   - Soft bounces: flag for retry in 48-72 hours

3. **VP presents report to CEO:**
   - Bounce count and rate by sequence
   - Enrichment results: how many recovered, how many dead ends
   - Recommended actions (re-enroll recovered contacts, remove dead ends)

4. **CEO APPROVAL CHECKPOINT** for re-enrollment

---

## PLAYBOOK 3: Gmail Signal Response

**Trigger**: Prospect replies to an email or engages in Gmail

### Signal Types and Auto-Responses

**"I'm interested in [event]"**
1. Sales Ops drafts enthusiastic follow-up with event details
2. Include registration info
3. Present to CEO for approval → send

**"Can't make [Event A] but interested in [Event B]"**
1. VP updates contact tags: target_event = [Event B]
2. VP removes from Event A sequence (if enrolled)
3. Sales Ops drafts Event B-specific follow-up
4. Present to CEO for approval → send
5. Queue for Event B sequence when it launches

**"Not interested" / "Remove me"**
1. VP flags for manual unsubscribe in HubSpot
2. Sales Ops drafts gracious acknowledgment (keep door open)
3. Remove from all active sequences
4. Present draft to CEO → send

**"Tell me more about [product]"**
1. Intelligence does quick research on their practice (if not already done)
2. Sales Ops drafts product-specific response tailored to their practice type
3. Include offer for demo or lunch meeting
4. Present to CEO for approval → send

**"I'd like to schedule a meeting"**
1. Sales Ops drafts confirmation email with meeting details placeholder
2. Describe what the calendar invite should contain
3. Present to CEO → CEO creates the calendar invite herself

**Referral: "Talk to Dr. X instead"**
1. Intelligence researches the referred contact
2. Sales Ops drafts outreach to the referral (crediting the referrer if appropriate)
3. Sales Ops drafts thank-you to the referrer
4. Check referral against exclusion list and territory
5. Present both drafts to CEO → send

---

## PLAYBOOK 4: New Territory Push

**Trigger**: "Let's start reaching out to [city/area]" or expanding into new part of territory

### Execution Steps
1. **Verify territory**: Confirm the area is in Aalia's assigned territory
2. **Intelligence builds prospect list:**
   - Pull contacts from HubSpot filtered by location
   - Enrich with ZoomInfo for missing data
   - Cross-reference exclusion list
   - Score and segment
3. **Intelligence provides market brief:**
   - How many practices in the area
   - Practice type breakdown
   - Any existing BTL presence (from exclusion list)
   - Competitive landscape if available
4. **VP recommends approach:**
   - Sequence type (event-focused, product-focused, or intro)
   - Suggested cadence and channel
   - Personalization tier based on prospect count
5. **CEO APPROVAL CHECKPOINT**
6. Execute using Playbook 1 or 2 as appropriate

---

## PLAYBOOK 5: Campaign Performance Review

**Trigger**: "How's the campaign doing?" or weekly/monthly check-in or proactively flagged

### Execution Steps
1. **Intelligence pulls data:**
   - Sequence metrics: enrolled, completed, bounced, replied
   - Email metrics: open rate, click rate, reply rate per email
   - Engagement breakdown: positive replies, questions, declines, opt-outs
   - Lead priority movement: who moved from Cold → Warm → Hot
2. **Intelligence produces report:**
   - Executive summary (3-5 key takeaways)
   - Performance by sequence
   - Top/bottom performing emails (subject lines, content)
   - Recommendations for optimization
3. **VP adds strategic context:**
   - What's working and should scale
   - What's not working and what to change
   - Cross-campaign patterns
4. **Present to CEO**

---

## PLAYBOOK 6: Post-Event Workflow

**Trigger**: Event just happened, or "Let's follow up on [event]"

### Execution Steps
1. **Intelligence segments attendees:**
   - Hot: expressed interest, asked about pricing/ordering
   - Warm: attended, engaged, but no commitment
   - Passive: showed up, minimal engagement
   - No-show: registered but didn't attend
2. **Marketing creates follow-up sequences** (using post-event-followup skill):
   - One sequence per segment with appropriate cadence and tone
   - Hot leads get fastest follow-up (same day)
   - No-shows get guilt-free "we missed you" + next event mention
3. **Sales Ops personalizes** where possible (reference specific conversations)
4. **VP assembles enrollment plan:**
   - Who goes into which sequence
   - Timing for each segment
5. **CEO APPROVAL CHECKPOINT**
6. Execute enrollment

---

## UNIVERSAL RULES (Apply to ALL Playbooks)

### Before Every Campaign
- [ ] Territory check passed
- [ ] Salesforce exclusion list cross-referenced
- [ ] No contacts currently in active sequences (unless CEO approves override)
- [ ] Confidentiality review: no speaker/vendor names without approval
- [ ] Email copy follows BTL style (no em dashes, warm tone, short paragraphs)
- [ ] CEO has approved before any execution

### Approval Levels
- **CEO must approve**: Any outreach that goes to a prospect, enrollment decisions, confidential content
- **VP can execute independently**: Internal analysis, research, data pulls, draft creation, enrichment recommendations
- **Department leads can execute independently**: Using their skills to create drafts (but not send)
