# AI Lead Qualification & Auto-Routing Agent

An AI-powered lead qualification and routing workflow built with **n8n and OpenAI**. It automatically captures incoming leads, analyzes their intent and urgency, classifies them as **Hot, Warm, or Cold**, and routes them to the appropriate follow-up actions.

## How It Works

1. A lead enters through an **n8n Webhook**.
2. JavaScript validates and structures the incoming data.
3. **OpenAI** analyzes the lead's intent and urgency.
4. The lead is classified as **Hot, Warm, or Cold**.
5. A personalized response is generated automatically.
6. The workflow routes the lead based on its classification:
   - 🔥 **Hot** → Slack alert + Gmail response + Google Sheets
   - 🌤️ **Warm** → Gmail response + Google Sheets
   - ❄️ **Cold** → Gmail response + Google Sheets

## Tech Stack

- **n8n** — Workflow automation and orchestration
- **OpenAI API** — AI classification and response generation
- **JavaScript** — Data validation and response parsing
- **Gmail** — Automated email responses
- **Google Sheets** — Lead logging and tracking
- **Slack** — Real-time Hot Lead alerts
- **Postman** — Webhook testing

## Why This Matters

This workflow demonstrates how AI-powered automation can streamline lead handling by classifying incoming inquiries, generating personalized responses, logging lead data, and routing high-priority opportunities automatically. It is designed to reduce repetitive lead screening and help teams respond to incoming opportunities more efficiently.


## Project Demo

Watch the full walkthrough(https://drive.google.com/file/d/1iYBxwj4XBWLoRd58I_ujPwAmJH9Mzk6B/view?usp=sharing)


## Built By

**Noor ul Ain**  
AI Automation Developer | n8n • AI Agents • RAG • API Integrations • Python
