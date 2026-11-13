# AI-Powered Social Media Growth Analyst

**Project 05 / 05 · Personal Automation Projects**

An AI-powered Instagram analytics automation workflow built with **n8n, Instagram Graph API, Google Gemini, JavaScript, and Gmail**.

The workflow automatically collects recent Instagram media, retrieves available post insights, processes performance metrics, uses Gemini AI to generate an analysis, and delivers the report through email.

## Overview

Manually reviewing individual social media posts can be time-consuming. This project explores how workflow automation and AI can help turn Instagram performance data into a structured, automatically delivered report.

### Workflow

```text
Weekly Trigger
     |
   Config
     |
Get Recent Media
     |
  Split Out
     |
 Get Post Insights
     |
 Compute Metrics
     |
 Gemini Analysis
     |
  Email Report
```

## How It Works

| Step | Node | Purpose |
|---|---|---|
| 1 | Weekly Trigger | Starts the workflow on a weekly schedule. |
| 2 | Config | Stores workflow configuration and analysis parameters. |
| 3 | Get Recent Media | Fetches recent Instagram media through the Instagram Graph API. |
| 4 | Split Out | Separates the media items for individual processing. |
| 5 | Get Post Insights | Retrieves available performance insights for each post. |
| 6 | Compute Metrics | Processes and organizes the collected data using JavaScript. |
| 7 | Gemini Analysis | Sends the processed information to Google Gemini for AI-powered analysis. |
| 8 | Email Report | Delivers the generated analysis through Gmail. |

## Technologies Used

- **n8n** — workflow orchestration and automation
- **Instagram Graph API** — Instagram media and insights retrieval
- **Google Gemini API** — AI-powered performance analysis
- **JavaScript** — data processing and metric calculations
- **HTTP Requests** — API communication and data handling
- **Gmail** — automated report delivery

## Repository Structure

```text
social-media-growth-analyst/
├── README.md
├── workflow/
│   └── social-media-growth-analyst.json
└── screenshots/
    ├── workflow-overview.png
    ├── instagram-data-collection.png
    ├── metrics-computation.png
    ├── gemini-analysis.png
    └── email-report.png
```

Add your exported n8n workflow JSON and genuine execution screenshots to the folders above. The filenames are suggested; adjust them to match the files you upload.

## Requirements

Before configuring the workflow, you will need:

- A running n8n instance
- An eligible Instagram professional account
- A Meta app and the required Instagram Graph API permissions and access token
- A Google Gemini API key
- A Gmail account connected to n8n

API access, permissions, available insights, and account eligibility depend on Meta's current platform requirements.

## Setup

1. Import the exported workflow JSON into your n8n instance.
2. Configure the weekly trigger and the values required by the Config node.
3. Connect your authorized Instagram Graph API credentials.
4. Verify the media retrieval and post-insights requests with your account.
5. Configure the JavaScript metrics-processing node for the fields returned by your API requests.
6. Connect your Google Gemini API credentials and review the analysis prompt.
7. Connect Gmail and configure the report recipient.
8. Test the workflow manually before enabling its weekly schedule.

**Important:** The workflow JSON and credentials are not included in this repository unless you add them yourself. Review every node and replace example values or placeholders before running it.

## Security

- Never upload API keys, access tokens, OAuth credentials, or exported credential data.
- Remove personal email addresses, private account identifiers, and other sensitive information from screenshots and sample outputs.
- Use n8n credentials or environment variables for secrets instead of hardcoding them in nodes.
- Review exported workflow JSON before publishing it. n8n exports can contain sensitive configuration values.

## Key Learnings

This project provided practical experience with:

- Multi-step API integrations
- Automated data collection
- Processing and organizing API responses
- JavaScript within automation workflows
- AI-powered analysis using Gemini
- Scheduled workflow execution
- Automated email reporting

**Main takeaway:** Collecting data is only one part of analytics. The real value comes from processing that data, understanding performance patterns, and turning the results into useful insights.

## Project Showcase

This project is part of my **Personal Automation Projects** series, where I explore practical applications of AI, APIs, backend concepts, and workflow automation.

---

**Built with n8n · Google Gemini · Instagram Graph API · JavaScript · Gmail**
