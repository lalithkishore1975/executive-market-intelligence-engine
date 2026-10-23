# Executive Market Intelligence Engine

An AI-powered competitor intelligence pipeline built with n8n that collects Google News RSS articles, processes and filters the data, generates a structured Tesla market intelligence briefing, and delivers it by email.

## Business Problem

Manually collecting competitor news and preparing regular intelligence reports takes time and can make it harder for decision-makers to track relevant developments consistently.

## Solution

This workflow automates news collection, article processing, AI-assisted analysis, and email reporting in a single pipeline.

## Workflow Architecture

1. **Schedule Trigger** — initiates the workflow.
2. **HTTP Request** — retrieves Google News RSS results.
3. **XML to JSON** — converts RSS data into structured records.
4. **JavaScript processing** — filters recent articles, removes duplicates, and prepares the records.
5. **AI analysis** — generates an executive briefing.
6. **JavaScript output processing** — parses the report and cleans source URLs.
7. **Gmail** — delivers the formatted report.

## Report Contents

- Executive summary
- Key competitor developments
- Potential opportunities and threats
- Recommended actions
- Evidence limitations and uncertainty

## Technology Stack

- n8n
- Google News RSS
- JavaScript
- AI language model
- Gmail

## Current Status

The workflow has successfully generated and delivered test reports. Findings depend on the number and quality of available RSS records; reports based on limited evidence should be treated as preliminary.

## Future Improvements

- Expand news-source coverage.
- Add workflow error notifications and recovery.
- Track competitor developments across multiple reporting periods.
- Evaluate report quality over time.

## Disclaimer

This is a portfolio project demonstrating workflow automation and AI-assisted market intelligence. The generated reports are analytical aids, not independently verified research or investment advice.
