# AI Customer Support Ticket Triage & Auto-Reply

An AI-powered customer support automation system built using n8n, Google Gemini, Gmail, and Google Sheets.

The workflow automatically analyzes incoming customer support tickets, determines their priority, routes them through different workflows, generates appropriate responses, sends emails to customers, and updates the support database.

---

## 🚀 Project Overview

Customer support teams often receive a large number of tickets that need to be categorized, prioritized, and answered.

This automation uses AI to analyze each incoming support ticket and determine how it should be handled.

The system can identify:

- Ticket priority
- Customer issue
- Support category
- Appropriate response
- Required workflow/action

Tickets are then routed according to their priority.

---

## 🧠 Workflow

```text
Google Sheets Trigger
        ↓
     AI Agent
        ↓
Update Ticket in Google Sheets
        ↓
      Switch
   ↙    ↓     ↘
HIGH   MEDIUM   LOW
 ↓       ↓       ↓
Gmail   AI Agent AI Agent
 ↓       ↓       ↓
Sheet   Gmail   Gmail
        ↓       ↓
       Sheet   Sheet
