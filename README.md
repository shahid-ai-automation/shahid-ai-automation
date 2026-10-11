# Shahid Abdullah

### AI Voice & Automation Engineer | Voice Agents · Smart Workflows · API Integrations

I build AI-powered voice experiences and the backend workflows that make them useful: structured customer conversations, requirement-aware property matching, appointment and viewing workflows, CRM updates, and business-system integrations.

My focus is on **reliable end-to-end automation**—not just connecting tools, but defining how data is collected, validated, routed, and turned into a confirmed business action.

- **Core focus:** Voice AI, AI agent workflows, backend APIs, workflow automation, CRM and calendar integrations
- **Current project focus:** Northstar Real Estate AI Receptionist & Smart Property Matching
- **Based around:** Python · FastAPI · Retell AI · n8n · Supabase/PostgreSQL · REST APIs

---

## Selected Work

### 01 — Northstar Real Estate AI Receptionist & Smart Property Matching

A real-estate voice-agent backend built around the Northstar demonstration business. The system connects a voice platform to a property API, a PostgreSQL-backed inventory, requirement-aware matching, and viewing workflows.

**What it covers**
- Property search by area, property type, bedrooms, listing type, and budget
- Smart matching that separates required, preferred, and flexible requirements
- Match explanations and a limited set of relevant property options
- Alternative recommendations when flexible criteria can be relaxed, without silently relaxing required criteria
- Viewing availability checks and booking workflows using Google Calendar
- Booking-related email notification workflows

**Architecture**

`Retell AI / Voice Agent → FastAPI → Supabase / PostgreSQL → Smart Matching`

`Availability & Booking → Google Calendar → Email Notification`

**Stack:** `Retell AI · Python · FastAPI · Supabase · PostgreSQL · REST APIs · Google Calendar · Gmail`

**Project links:** [Backend repository](https://github.com/shahid-ai-automation/ai-voice-sales-agent) · [Northstar Property API repository](https://github.com/shahid-ai-automation/northstar-property-api) · [Live API documentation](https://northstar-property-api-production.up.railway.app/docs) · [Health check](https://northstar-property-api-production.up.railway.app/)

*Status: Public demonstration deployment. The backend documents known production-readiness limitations; it should not be treated as a hardened production service for real customer bookings yet.*

---

### 02 — BrightSmile Dental Clinic AI Voice Receptionist

A clinic receptionist workflow designed to connect a voice conversation to the appointment and follow-up process, rather than leaving the call as a standalone interaction.

**Workflow**

`Voice Call → Availability Check → Appointment Booking → Google Calendar → Google Sheets → HubSpot → Email`

**What it covers**
- Appointment availability and booking workflows
- Appointment lookup and cancellation flows
- Call-related data capture and follow-up automation
- Contact and deal updates in HubSpot

**Stack:** `Retell AI · n8n · Google Calendar · Google Sheets · HubSpot · Email`

[View the project demo on LinkedIn](https://www.linkedin.com/posts/shahid-ai-automation_aiautomation-voiceai-n8n-activity-7493581816474398721-MmT8)

---

### 03 — Lead Generation & HubSpot Automation

An end-to-end lead workflow for prospect discovery, qualification, enrichment, CRM ingestion, and score-based segmentation.

**Workflow**

`Prospect Discovery → Qualification → Enrichment → Google Sheets → HubSpot → Lead Scoring → Segmentation → Targeted Outreach`

**Focus areas**
- Structured lead records and qualification signals
- Contact and business-data enrichment
- HubSpot contact organization and lead scoring
- Segmentation into different follow-up paths

[View the workflow repository documentation](./lead-generation-hubspot-automation/README.md) · [Lead workflow on LinkedIn](https://www.linkedin.com/posts/shahid-ai-automation_i-built-a-lead-scraping-and-scoring-workflow-activity-7494056832295141376-YGrN) · [HubSpot segmentation on LinkedIn](https://www.linkedin.com/posts/shahid-ai-automation_from-lead-generation-to-targeted-outreach-activity-7495459752353742850-G3db)

---

## Tools & Technologies

| Area | Tools |
|---|---|
| **Voice AI & agents** | Retell AI · Vapi AI · LiveKit |
| **Workflow automation** | n8n · Webhooks · Event-driven workflows |
| **Backend & APIs** | Python · FastAPI · REST APIs · JSON · API authentication |
| **Data & storage** | PostgreSQL · Supabase · Google Sheets |
| **CRM & business systems** | HubSpot · Google Calendar · Gmail |
| **Integration patterns** | HTTP requests · API tools · Structured payloads · Third-party service integration |

*Tools are used across different projects; they are not all part of every project. Project-specific stacks are listed in each case study.*

---

## How I Approach Automation

I start with the business process, then design the integration around it.

1. **Capture the request** — identify the customer's intent and required information.
2. **Validate the data** — distinguish confirmed requirements from assumptions.
3. **Apply business rules** — search, match, qualify, or check availability using defined logic.
4. **Call the right system** — connect APIs, calendars, databases, and CRMs.
5. **Verify the outcome** — only report a booking, match, or completed action when the relevant system confirms it.
6. **Keep the workflow maintainable** — separate responsibilities so individual steps can evolve without rebuilding everything.

This approach helps keep AI conversations connected to reliable business operations.

---

## Current Focus

- Voice agents connected to real backend tools
- Requirement-aware search and smart matching
- Appointment and property-viewing workflows
- Secure API integrations and validation
- Reusable automation patterns across voice, CRM, and business systems

## Contact

- **LinkedIn:** [Shahid Abdullah](https://www.linkedin.com/in/shahid-ai-automation/)
- **GitHub:** [shahid-ai-automation](https://github.com/shahid-ai-automation)
