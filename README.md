# AI Lead Qualification & Auto-Routing Agent

An automation built with **n8n** and the **OpenAI API** that reads incoming lead
inquiries, uses AI to classify them as Hot, Warm, or Cold, and automatically
routes each one to the right action — with zero manual work.

## What It Does

1. A new lead submits an inquiry (via API/webhook).
2. An AI model reads the message and classifies it as **Hot**, **Warm**, or **Cold**,
   based on urgency and clarity of intent.
3. The AI also drafts a short, personalized reply for that specific lead.
4. Based on the classification, the system automatically:
   - Logs every lead into a tracking spreadsheet
   - Sends the AI-generated personalized reply to the lead's email
   - Sends an instant Slack alert **only** for Hot leads, so nothing urgent is missed

## Tech Stack

- **n8n** — workflow orchestration and automation logic
- **OpenAI API** — lead classification and personalized reply generation
- **Google Sheets** — lead logging / CRM-style tracking
- **Gmail** — automated personalized email replies
- **Slack** — real-time alerts for high-priority leads
- **Postman** — used for testing the webhook/API integration during development

## Architecture

Webhook (receives lead data)
→ Validation (Code node)
→ AI Classification (OpenAI)
→ Response Parsing (Code node)
→ Switch (routes by Hot / Warm / Cold)
├── Hot → Slack Alert + Sheet Log + Email Reply
├── Warm → Sheet Log + Email Reply
└── Cold → Sheet Log + Email Reply

## Demo

Watch the full walkthrough(LINK_HERE)

## Why This Matters

Small businesses lose leads every day simply because no one follows up fast
enough. This automation removes that gap entirely leads are read, judged,
logged, and responded to within seconds of coming in, with zero manual effort
from the business owner.
