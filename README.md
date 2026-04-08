# Salesforce Gig Income Tracker

A custom Salesforce developer org built to track Uber and DoorDash income at the trip level — with dashboards, automation, and a Lightning Web Component for fast data entry.

## The Problem

Gig platforms give drivers aggregate summaries but no easy way to analyze earnings by trip, day, platform, or time of day. Understanding which hours are most profitable, what tip percentages look like across platforms, or how weekly income trends over time requires either a spreadsheet built from scratch or a CRM built for it.

## What I Built

A Salesforce developer org with a custom data model, dashboards, and a Lightning Web Component — designed specifically around gig income tracking. Every trip becomes a structured record with fields that Uber and DoorDash don't surface natively.

## Data Model

**Custom Object: `Income_Record__c`**

| Field | Description |
|-------|-------------|
| Base Fare | Platform base pay for the trip |
| Surge / Promotion | Additional platform pay |
| Tip | Customer tip amount |
| Miles | Trip distance |
| Time Taken | Duration of the trip |
| Net Income | Calculated total |
| Platform | Uber or DoorDash |

## Features

- **Dashboard:** Current week and month income totals, tip percentage breakdowns by platform
- **Lightning Web Component (LWC):** Custom quick-entry form embedded on the Salesforce home page for fast manual record creation
- **Automated ingestion:** [Pixit](https://usepixit.com) extracts trip data from screenshots and creates `Income_Record__c` records automatically via sf CLI — no manual entry required when using the full pipeline
- **Reports:** Earnings by platform, time period, and tip rate

## Tech Stack

- Salesforce (Developer Org)
- Lightning Web Components (LWC)
- Salesforce CLI (sf CLI) for record creation via external automation
- SOQL for report logic
- Connected to Pixit (Node.js app) for automated data ingestion

## Certifications & Training

- Salesforce Administrator Certified
- Salesforce Associate Certified
- 12-week APEX Developer course
- Hands-on experience with Flows, LWC, custom objects, dashboards, and external integrations

## What I Learned

- Designing a custom data model for a real-world use case from scratch
- Building a Lightning Web Component for a custom home page UI
- Connecting an external application (Pixit) to Salesforce via CLI auth
- Using Reports and Dashboards to surface actionable business insights from raw data
- How CRM concepts apply to non-traditional use cases (gig economy income tracking)

## Status

Functional and actively used as my primary income tracking tool. Serves as both a practical application and a live demonstration of Salesforce development skills.
