# Lead Generation & HubSpot Lead Scoring Automation

An automation pipeline built to take targeted prospects from initial research to **qualified, enriched CRM records and score-based segmentation**.

This project combines two workflows I built and shared separately on LinkedIn, but presents them here as one operational pipeline.

---

## System Flow

```text
Prospect Discovery
      ↓
Lead Qualification & Scoring
      ↓
Email + Social Enrichment
      ↓
Google Sheets
      ↓
HubSpot CRM
      ↓
Score-Based Segmentation
      ↓
Targeted Outreach / Nurturing
```

The important part of the workflow is the handoff between stages: the output of lead research becomes structured CRM input, and the qualification data is then used to determine how each lead should be handled.

---

## 01 — Lead Generation, Qualification & Enrichment

The first workflow was designed to make prospect research repeatable instead of manually compiling lead lists one record at a time.

### Process

- Identify businesses matching the target criteria
- Collect prospect and company information
- Evaluate leads against qualification signals
- Calculate a lead score
- Enrich records with available business email information
- Collect relevant social profiles
- Write the qualified dataset into Google Sheets

### Lead Record

The resulting sheet is structured around information that can be used downstream, including:

- Company / business
- Contact information
- Website
- Business email
- Social profiles
- Qualification signals
- Lead score

**LinkedIn project:**

[View Lead Scraping & Scoring Workflow](https://www.linkedin.com/posts/shahid-ai-automation_i-built-a-lead-scraping-and-scoring-workflow-activity-7494056832295141376-YGrN)

---

## 02 — HubSpot CRM Ingestion & Score-Based Segmentation

The second workflow starts with the qualified Google Sheets dataset.

Leads are transferred into HubSpot and organized using their qualification scores. Instead of putting every contact into the same follow-up path, the workflow uses the score to determine the appropriate segment.

```text
Qualified Lead
      ↓
HubSpot Contact
      ↓
Lead Score
      ↓
┌──────────────┬──────────────┬──────────────┐
│ High Score   │ Medium Score │ Low Score    │
│ Priority     │ Nurture      │ Long-Term    │
│ Outreach     │              │ Nurture      │
└──────────────┴──────────────┴──────────────┘
```

This creates a practical separation between **sales-ready prospects and leads that require further nurturing**.

**LinkedIn project:**

[View HubSpot Segmentation & Targeted Outreach Workflow](https://www.linkedin.com/posts/shahid-ai-automation_from-lead-generation-to-targeted-outreach-activity-7495459752353742850-G3db)

---

## Automation Stack

| Component | Role |
|---|---|
| **n8n** | Workflow orchestration and data movement |
| **Lead scraping / research tools** | Prospect discovery and initial data collection |
| **Google Sheets** | Qualified lead staging and structured handoff |
| **HubSpot** | CRM records, scoring and segmentation |
| **APIs / Webhooks** | Integration between workflow stages |

---

## Why the Architecture Matters

A lead list is only useful when the information collected can drive the next action.

This workflow separates the process into clear operational stages:

**Research → Qualification → Enrichment → CRM → Scoring → Segmentation → Outreach**

That structure makes it possible to change the lead source, qualification rules, enrichment process, or CRM logic without rebuilding the entire pipeline.

---

## Implementation Focus

- Structured lead data rather than unorganized scraped output
- Qualification before CRM ingestion
- Score-driven prioritization
- Automated CRM segmentation
- Clear handoff between prospecting and CRM operations
- Reduced manual lead preparation and classification
- A workflow designed around downstream sales actions, not just data collection

---

## Project Scope

This repository documents the **automation architecture and business workflow**. Credentials, private CRM data, and production contact records are intentionally excluded.
