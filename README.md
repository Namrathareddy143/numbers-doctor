# 🩺 Numbers Doctor: Dashboard Trust Agent

An AI agent built in **n8n** that investigates why a BI dashboard number doesn't match its source, and shows the evidence behind every diagnosis.

> "The dashboard says 1.2M, the source says 1.15M. Which one is right?" Numbers Doctor answers that question.

## The problem
Business users lose trust in dashboards when numbers don't match the source system. Analysts then spend hours digging through refresh logs, filters and raw data to find out why.

## How it works
1. A dashboard KPI is compared with its source data.
2. When they differ, the AI agent investigates using 3 tools:
   - 🔍 **Drill-down**: finds which segment or period causes the gap
   - 🕒 **Refresh-log check**: finds stale or failed refreshes
   - 🧾 **Duplicate/missing check**: finds duplicated or missing records
3. The agent returns a diagnosis **with the evidence** behind it.
4. A **Email approval flow (Approve / Decline)** asks a human to approve before any action is taken.

## Tech stack
- n8n (workflow and AI agent)
- [LLM used, e.g. OpenAI / Gemini]
- Email (approvals)
- [Data source: Google Sheets
SAC support is designed as an optional adapter. CSV/Power BI is the default.

## Demo
[Add screenshot or GIF here]
[Link to demo video]

## How to run
1. Import `Numbers Doctor v2 - Dashboard Trust Agent.json` into n8n (*Workflows → Import from file*).
2. Add your own credentials (LLM API key, Email bot).
3. Add the sample data and run the workflow.

## About me
I'm [your name], building toward a career in SAP Analytics Cloud and BI.
Connect with me on [LinkedIn link].

## License
MIT
