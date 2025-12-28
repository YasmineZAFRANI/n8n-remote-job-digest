# n8n-remote-job-digest
This project showcases how I design end-to-end data workflows using n8n, from ingestion to scoring and delivery, with a clear path toward production-grade architecture.

# n8n Remote Job Digest & Scoring

Automated n8n workflow that fetches remote job offers, filters and scores them
for EU/FR relevance, and sends a prioritized email digest.

## Overview
This workflow:
- Retrieves job offers from RemoteOK (and RSS-compatible sources)
- Normalizes heterogeneous job data
- Filters offers based on role relevance and EU/France location
- Applies a scoring logic to prioritize the most relevant jobs
- Stores results in a job tracker
- Sends an automated email digest

## Workflow Steps
1. Scheduled trigger
2. API / RSS ingestion
3. Data normalization
4. Filtering & scoring logic
5. Job tracking
6. Email digest delivery

## Tech Stack
- n8n
- REST APIs (RemoteOK)
- JavaScript (n8n Function nodes)
- Google Sheets (job tracking)
- Email service

## Scoring Logic (Summary)
Jobs are scored based on:
- Role relevance (Data / BI / Analytics)
- EU / France location
- Remote eligibility
- Keyword matching (Python, SQL, BI tools)

Only high-relevance jobs are included in the final digest.

## Future Improvements
See the **Project Roadmap** section below.
