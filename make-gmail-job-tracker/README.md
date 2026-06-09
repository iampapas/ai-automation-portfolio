# Make.com — Gmail Job Tracker Pipeline

**Built by:** Jennifer Ugarte | Ugarte Consulting

## What It Does
A multi-step automation pipeline that watches a Gmail inbox for 
job-related emails, uses Claude (Anthropic) to classify and summarize 
each email, and logs structured output to Google Sheets for later review.

## How It Works
1. Gmail module watches inbox for incoming emails
2. Filter module screens for job-related content
3. Claude AI module classifies email into categories:
   Interview Request | Recruiter Outreach | Application Confirmation | 
   Rejection | Job Offer | Follow Up | Other
4. Claude generates a one-sentence summary of each email
5. Google Sheets module logs category, summary, sender, and date

## Why I Built It
Manual inbox management during an active job search is time-consuming. 
This pipeline automates classification and logging so nothing falls 
through the cracks.

## Tech Stack
- Make.com
- Gmail API (via Make.com connector)
- Anthropic Claude API (via Make.com HTTP module)
- Google Sheets

## Status
Live and running in production daily.
