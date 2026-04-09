# BTL Marketing Team — Organizational Structure

## The Hierarchy

```
CEO — Aalia Mohammad
  ├── VP of Sales & Marketing — Sales Dev Agent (always-on coordinator)
  └── CTO — Engineering Coordinator (always-on, owns all technical systems)
        ├── SALES OPERATIONS DEPARTMENT
        │     ├── Director: Outreach Specialist (owns all email/sequence execution)
        │     └── Skills:
        │           ├── Email Sequence Writer
        │           ├── Follow-Up Drafter
        │           └── Sales Outreach Composer
        │
        ├── MARKETING DEPARTMENT
        │     ├── Director: Event Campaign Manager (owns events + content strategy)
        │     ├── Skills:
        │     │     ├── Event Invite Creator
        │     │     ├── Event Reminder Sequence
        │     │     └── Post-Event Follow-Up
        │     └── Reports to Director:
        │           └── Content Creator (agent — blog, social, landing pages)
        │                 ├── Blog Writer (skill)
        │                 ├── Social Post Creator (skill)
        │                 └── Landing Page Builder (skill)
        │
        ├── INTELLIGENCE DEPARTMENT
        │     ├── Director: Research Analyst (owns prospect research + market intel)
        │     └── Skills:
        │           ├── Prospect Research
        │           ├── Contact Enrichment
        │           └── Campaign Report
        │
        └── REVOPS DEPARTMENT
              ├── Director: RevOps Manager (owns HubSpot health + data hygiene)
              └── Skills:
                    ├── HubSpot Data Cleanup
                    ├── Sequence Audit
                    └── Contact Import Prep
        │
        └── ENGINEERING DEPARTMENT
              ├── CTO (Director — coordinates all technical work)
              ├── Frontend Engineer (dashboard UI, GitHub Pages)
              ├── Backend Engineer (API integrations, data pipelines)
              └── DevOps Engineer (CI/CD, GitHub Actions, 24/7 automation)
```

## Total Team Size: 10 Agents + 15 Skills

| # | Agent | Role | Department | Skills |
|---|-------|------|------------|--------|
| 1 | Sales Dev Agent | VP / Always-on Coordinator | Executive | Coordinates all departments |
| 2 | Outreach Specialist | Director of Sales Ops | Sales Operations | 3 skills |
| 3 | Event Campaign Manager | Director of Marketing | Marketing | 3 skills + manages Content Creator |
| 4 | Content Creator | Marketing Specialist | Marketing (reports to ECM) | 3 skills |
| 5 | Research Analyst | Director of Intelligence | Intelligence | 3 skills |
| 6 | RevOps Manager | Director of RevOps | RevOps | 3 skills |
| 7 | CTO | Engineering Coordinator | Engineering | Coordinates engineers |
| 8 | Frontend Engineer | UI/Dashboard Builder | Engineering | dashboard-builder, component-builder |
| 9 | Backend Engineer | Integrations & Data | Engineering | api-integration, data-pipeline |
| 10 | DevOps Engineer | CI/CD & Automation | Engineering | github-actions-builder, cron-scheduler |

## How It Flows

### CEO (Aalia)
- Sets strategic direction ("Focus on Dallas this week")
- Approves all outreach before it goes live
- Reviews confidential content
- Makes final calls on edge cases (territory, exclusions)
- Provides brand assets, flyers, and templates (agents don't create flyers — Aalia has pre-made ones)

### VP of Sales & Marketing (Sales Dev Agent)
- Receives ALL tasks from the CEO — single point of entry
- Breaks complex tasks into department-level assignments
- Coordinates cross-department work
- Runs proactively: monitors HubSpot, Gmail, flags issues
- Assembles final deliverables for CEO approval
- Enforces all operational rules (territory, exclusions, confidentiality)

### Sales Operations Department
**Director: Outreach Specialist**
- Owns all email copy and sequence creation
- Handles reply responses and follow-ups
- Manages HubSpot sequence enrollment recommendations
- Uses: email-sequence-writer, follow-up-drafter, sales-outreach-composer

### Marketing Department
**Director: Event Campaign Manager**
- Owns the full event lifecycle for Tulsa and Dallas
- Manages the Content Creator for supporting materials
- Coordinates event branding (Modern Medicine Symposium vs. Art of the Eyes)
- NOTE: Does NOT create flyers or design assets — Aalia provides pre-made flyers. Marketing writes the messaging and email copy around those assets.
- Uses: event-invite-creator, event-reminder-sequence, post-event-followup

**Content Creator (reports to Event Campaign Manager)**
- Produces blog posts, social media, landing pages, lead magnets
- Takes direction from the Event Campaign Manager for event-supporting content
- Can also be tasked directly by the VP for non-event content
- Uses: blog-writer, social-post-creator, landing-page-builder

### Intelligence Department
**Director: Research Analyst**
- Owns prospect research and market intelligence (outward-facing)
- Finds new prospects via ZoomInfo, web research
- Provides intel to Sales Ops before outreach campaigns
- Produces campaign performance reports
- Uses: prospect-research, contact-enrichment, campaign-report

### RevOps Department
**Director: RevOps Manager**
- Owns HubSpot system health (inward-facing)
- Contact data hygiene: deduplication, bounce cleanup, missing data identification
- Sequence auditing: performance monitoring, junk task detection, threshold analysis
- Import operations: cleans new CSVs, deduplicates against HubSpot, preps for import
- Property management: ensures custom properties are populated and consistent
- Workflow monitoring: checks that automations are firing correctly
- Uses: hubspot-data-cleanup, sequence-audit, contact-import-prep

## Cross-Department Workflows

### "Let's run a Dallas event sequence"
1. VP receives task from CEO
2. VP tasks RevOps → Audit current data health, ensure contacts are clean
3. VP tasks Intelligence → Pull qualified contacts, filter by territory + exclusions
4. VP tasks Marketing → Write invite messaging (using Aalia's pre-made flyers as reference)
5. VP tasks Sales Ops → Draft the email sequence using Marketing's messaging
6. VP assembles everything: filtered contact list + sequence copy + enrollment plan
7. VP presents to CEO for confidentiality review and approval
8. CEO approves → VP coordinates execution
9. RevOps monitors sequence health post-launch

### "Here's a new contact list" (CSV import)
1. VP receives file from CEO
2. VP tasks RevOps → Contact Import Prep runs the full pipeline:
   - Clean data → deduplicate → territory filter → exclusion filter → property mapping
3. RevOps presents import report to VP
4. VP presents to CEO with summary: "[X] contacts ready to import, [Y] removed, here's why"
5. CEO approves → RevOps executes import
6. Intelligence scores and segments the new contacts
7. Sales Ops queues them for appropriate outreach

### "Find me more contacts in Midland"
1. VP receives task from CEO
2. VP tasks Intelligence → Research Analyst uses ZoomInfo to find practices in Midland/Odessa area
3. Intelligence delivers raw prospect list
4. VP tasks RevOps → Clean the list, deduplicate against HubSpot, run territory + exclusion filters
5. VP presents: "[X] new prospects found, [Y] ready to import after filtering"
6. CEO approves → RevOps imports, Intelligence scores, Sales Ops builds outreach plan

### "How are our sequences doing?"
1. VP receives task from CEO
2. VP tasks RevOps → Sequence Audit runs across all active sequences
3. RevOps delivers health report: bounce rates, engagement metrics, junk task detection
4. VP tasks Intelligence → Campaign Report with strategic analysis and recommendations
5. VP presents combined report to CEO with action items

## Model Routing
- **VP (Sales Dev)**: Primary model — full reasoning for coordination
- **Sales Ops (Outreach Specialist)**: Can use faster model for straightforward email drafts
- **Marketing (Event Campaign Manager + Content Creator)**: Primary model for creative work
- **Intelligence (Research Analyst)**: Primary model for analysis and research
- **RevOps (RevOps Manager)**: Primary model for data operations and auditing
