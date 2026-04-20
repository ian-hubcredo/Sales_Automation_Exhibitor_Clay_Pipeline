# SA Flow 2

## Overview

An updated version of the SA Flow conference exhibitor lead generation pipeline. It adds Clay integration for lead enrichment and includes refined ICP filtering with additional data cleaning steps. The core flow remains the same: scrape exhibitors from MapYourShow, find domains via AI, enrich through Apollo, filter by ICP, find decision-makers, verify emails, and push to outreach campaigns.

## How It Works

```
Form (event URL) -> Apify MapYourShow Scraper -> Clean data -> AI find domains -> Apollo Org Enrichment -> ICP Filter -> Apollo People Search -> Clean + Save to Sheet -> Push to Clay -> Aimfox + Instantly campaigns
```

## Integrations

- **Apify** - MapYourShow exhibitor scraping
- **OpenAI** - Domain research
- **Apollo** - Organization enrichment and people search
- **Google Sheets** - Lead storage
- **Clay** - Lead enrichment
- **Aimfox** - LinkedIn outreach
- **Instantly** - Email outreach

## Setup

1. Import `SA_Flow_2.json` into your n8n instance.
2. Configure all credentials.
3. Activate and submit the form with an event URL.
