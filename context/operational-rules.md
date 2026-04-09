# BTL Marketing Team — Operational Rules

These rules apply to ALL agents and ALL outreach. They are non-negotiable and must be checked before any external communication is sent.

---

## 1. Territory Restrictions

### Approved Territory
- **Oklahoma**: Full state — all cities and regions
- **Texas (partial)**: Only Aalia's assigned regions:
  - North Texas / Dallas-Fort Worth metro area
  - West Texas: Midland, Odessa, and surrounding areas
  - Specific boundaries to be confirmed with Aalia's account list

### Off-Limits
- Any state outside OK and TX
- Texas regions outside Aalia's assigned territory
- If a contact's location is ambiguous or borderline → ASK Aalia before including

### How to Verify
- Check the contact's city/state in HubSpot
- Cross-reference against the territory map (to be provided)
- When in doubt, flag for review

---

## 2. Salesforce Exclusion List (Do Not Contact)

### Purpose
BTL practices that already have devices and/or an assigned Practice Success Manager are managed by their PSM. Cold outreach to these accounts would be stepping on a colleague's territory.

### Rules
- Before ANY outreach: cross-reference every contact against the exclusion list
- Match by **practice name** (primary) and **contact email domain** (secondary)
- If a practice appears on the exclusion list → **DO NOT CONTACT** under any circumstance
- If uncertain → **FLAG for Aalia**, do not proceed

### Exclusion List Location
`context/salesforce-exclusions/` — Aalia will populate this with a Salesforce export

### Updating the List
- Aalia will provide updated exports periodically
- Always use the most recent version
- If the list hasn't been updated in 30+ days, remind Aalia

---

## 3. Confidentiality Protocol

### Why This Matters
BTL is a secretive company. Competitors (InMode, CoolSculpting, etc.) actively monitor for intelligence about BTL's events, partnerships, and strategy. Any leak of speaker names, vendor names, or proprietary details gives competitors an advantage.

### NEVER Share Without Explicit Approval
- Speaker names or bios
- Vendor names or partnerships
- Specific agenda items, session titles, or curriculum details
- Internal BTL strategies, pricing, or roadmap information
- Partner company names
- Names of practices that have purchased BTL devices

### Safe to Share (Default — unless Aalia restricts)
- Event name (The Modern Medicine Symposium / The Art of the Eyes)
- Event dates and location/venue
- General themes: "hands-on training," "CE credits," "networking with peers"
- Registration link or instructions
- That the event is complimentary / free to attend
- General product categories (body contouring, facial treatments, etc.)

### Mandatory Review Process
1. Before any campaign launch, present ALL outreach copy to Aalia
2. Aalia will mark what's approved to share for that specific campaign
3. Do not reuse approvals from past campaigns — each campaign gets fresh review
4. If in doubt about whether something is confidential → it IS confidential

---

## 4. HubSpot Sequence Rules

### One Sequence Per Contact
- HubSpot allows only ONE active sequence per contact
- Before enrolling: verify the contact is not already in an active sequence
- If they are: get Aalia's approval before unenrolling/re-enrolling

### Sequence Signal Threshold
- Current threshold: "2 opens or 1 click" — but this has caused issues with bot opens creating junk tasks
- Be aware of this when analyzing engagement data
- True engagement signals: replies, link clicks to specific pages, registration form submissions

### Bounce Handling
- If a contact bounces → do NOT re-enroll in another sequence
- Instead: flag for enrichment (find updated email via ZoomInfo or web research)
- Track bounce rates per sequence — if >5%, escalate

---

## 5. Communication Standards

### Email Style (applies to all agents)
- Warm, low-pressure, peer-level tone
- NO em dashes (—) anywhere in body copy
- Short paragraphs (2-3 sentences max)
- General office emails: "Hi there" (not a specific name)
- Named contacts: first name only
- Meeting framing: "bring lunch to the office" or virtual. NEVER "grab lunch"
- Attribution: only reference conversations that actually happened with the actual person
- Always mention both events when applicable (Tulsa + Dallas)
- Signature: Aalia Mohammad | Practice Success Manager | [phone] | [email]

### Reply Handling
- "Re:" prefix must match original thread subject exactly
- Positive replies → fast, enthusiastic but not pushy response
- Declines → gracious, keep door open, mention alternative event
- Opt-outs → flag for manual unsubscribe (HubSpot can't auto-detect)
- Event switches ("can't do Tulsa but Dallas works") → tag for alternate event, adjust sequence

### Calendar Events
- NEVER auto-create calendar events
- Draft confirmation email with meeting link placeholder
- Aalia creates all calendar invites herself

---

## 6. Approval Workflow

### Requires Aalia's Approval Before Execution
- Any new outreach campaign or sequence launch
- Event email copy (confidentiality review)
- Enrollment of contacts into sequences
- Unenrolling contacts from active sequences
- Any communication to a contact that's borderline (territory, exclusion list)
- SMS messages (when Twilio is active)

### Can Execute Without Approval
- Data analysis and reporting
- Research and enrichment recommendations
- Drafting (but not sending) email copy
- Flagging issues and opportunities
- Updating internal tracking documents

---

## 7. Data Sources and Trust Hierarchy

When information conflicts, trust in this order:
1. **Aalia's direct instructions** (highest authority)
2. **Salesforce exclusion list** (for account-level decisions)
3. **HubSpot CRM data** (for contact-level details)
4. **Gmail threads** (for conversation context and signals)
5. **ZoomInfo enrichment** (for supplementary data)
6. **Web research** (lowest — verify before acting on it)
