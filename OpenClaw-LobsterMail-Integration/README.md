# OpenClaw + LobsterMail Integration Guide

## What This Does

Give your OpenClaw AI agent its own email address to send and receive emails autonomously. Perfect for real estate lead follow-up, client communication, and automated workflows.

## Why LobsterMail

- **$9/month** (vs AgentMail $20+)
- **Unlimited inboxes** on Builder plan
- **Built-in prompt injection protection**
- Simple API, great docs

---

## Prerequisites

1. OpenClaw installed and running
2. LobsterMail account (sign up at lobstermail.ai)
3. API key from LobsterMail dashboard

---

## Step 1: Get LobsterMail API Key

1. Go to [lobstermail.ai](https://lobstermail.ai)
2. Sign up for free account
3. Go to Dashboard → API Keys
4. Copy your API key

---

## Step 2: Create an Inbox for Your Agent

```bash
# API call to create inbox
curl -X POST "https://api.lobstermail.ai/v1/inboxes" \
  -H "Authorization: YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "name": "realestate-assistant",
    "description": "OpenClaw real estate agent assistant"
  }'
```

Response:
```json
{
  "id": "inbox_abc123",
  "email": "realestate-assistant@lobstermail.ai",
  "status": "active"
}
```

---

## Step 3: Configure OpenClaw

Add to your OpenClaw config:

```json
{
  "channels": {
    "email": {
      "enabled": true,
      "provider": "lobstermail",
      "apiKey": "YOUR_LOBSTERMAIL_API_KEY",
      "inboxId": "inbox_abc123",
      "fromEmail": "realestate-assistant@lobstermail.ai"
    }
  },
  "agents": {
    "realestate": {
      "channels": ["discord", "email"],
      "tools": {
        "allow": ["email", "calendar", "search"]
      }
    }
  }
}
```

---

## Step 4: Test It

Send a test email through your agent:

```
Send an email to yourself@lobster.com with subject "Test" and body "Hello from your AI agent!"
```

The agent should send the email and you should receive it.

---

## What Your Agent Can Now Do

✅ **Lead Response** - Auto-reply to new leads within minutes  
✅ **Follow-Up Sequences** - Automated follow-ups after showings  
✅ **Property Alerts** - Send new listings to matching buyers  
✅ **Market Updates** - Weekly newsletter to your sphere  

---

## Cost

| Item | Monthly Cost |
|------|--------------|
| LobsterMail Builder | $9 |
| OpenClaw (your setup) | $0-20 |
| OpenAI API | $5-20 |
| **Total** | **$14-29/month** |

---

## Troubleshooting

### Emails not sending?
- Verify API key is correct
- Check inbox is active (not suspended)
- Make sure you're on Builder plan for sending

### Agent not reading emails?
- Check webhooks are configured
- Verify inbox ID matches

### Rate limits?
- Free plan: 1,000 emails/month
- Builder plan: Unlimited

---

## Example Real Estate Workflow

```
Trigger: New lead enters CRM
↓
Agent sends: "Hi [Name], thanks for reaching out! Tell me about what you're looking for..."
↓
Lead replies: "Need 3BR in Austin under $450k"
↓
Agent qualifies: Asks budget, timeline, location preferences
↓
Agent logs: Lead details saved to spreadsheet
↓
Agent schedules: Call with agent for tomorrow 2pm
```

All automated via email!

---

## Next Steps

1. Test with the Free tier (1,000 emails/month)
2. Upgrade to Builder ($9) for unlimited
3. Create workflows for your specific niche
4. Monetize by selling the automation to others

---

*For support, check LobsterMail docs or OpenClaw community.*