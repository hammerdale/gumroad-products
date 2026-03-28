# OpenClaw Real Estate Workflow - Setup Guide

## Prerequisites

Before starting, you'll need:

1. **OpenClaw installed** - See [OpenClaw Docs](https://docs.openclaw.ai)
2. **OpenAI API key** - Get at [platform.openai.com](https://platform.openai.com) ($5-10/month)
3. **Discord bot** - Create at [discord.com/developers](https://discord.com/developers)
4. **Gmail account** (optional) - For automated emails

---

## Step 1: Install OpenClaw

```bash
# On your machine
curl -sL https://openclaw.ai/install | bash
```

Or follow the detailed guide at https://docs.openclaw.ai

---

## Step 2: Configure Your Agent

Open your OpenClaw config:
```bash
openclaw config edit
```

Add this configuration:

```json
{
  "agents": {
    "realestate": {
      "model": "openai/gpt-4",
      "systemPrompt": "system-prompt.md",
      "channels": ["discord"],
      "tools": {
        "allow": ["email", "calendar", "search"]
      }
    }
  }
}
```

---

## Step 3: Set Up Discord Bot

1. Create a Discord application at developer portal
2. Add a bot user
3. Enable Message Content Intent
4. Get the bot token
5. Add to your server

Configure in OpenClaw:
```bash
openclaw config set channels.discord.token "YOUR_TOKEN"
```

---

## Step 4: Add Your API Keys

```bash
# OpenAI API key
export OPENAI_API_KEY="sk-..."

# Or Anthropic (optional)
export ANTHROPIC_API_KEY="sk-ant-..."
```

---

## Step 5: Test the Workflow

1. Start your agent:
```bash
openclaw start realestate
```

2. Send a test message in Discord:
```
Hi! I'm looking for a 3BR home in Austin, TX under $500k.
```

3. The agent should respond within 30 seconds with qualifying questions.

---

## Step 6: Customize for Your Business

Edit `system-prompt.md` to add:
- Your name and license number
- Your specific contact info
- Your local market knowledge
- Any specialized areas (luxury, first-time buyers, etc.)

---

## Troubleshooting

### Agent not responding?
- Check OpenClaw logs: `openclaw logs`
- Verify API keys are set
- Check Discord bot is online

### Wrong responses?
- Edit system prompt with more specific instructions
- Add example conversations in the prompt

### Not sending emails?
- Verify Gmail SMTP settings
- Check that email tool is enabled

---

## Cost Estimate

| Item | Monthly Cost |
|------|--------------|
| OpenAI GPT-4 | $5-20 |
| Discord bot | Free |
| OpenClaw hosting (VPS) | $5-20 |
| **Total** | **$10-40/month** |

---

## Next Steps

Once running, you can:
- Add more skills (SMS, voice calls)
- Connect to CRM (Salesforce, HubSpot)
- Add listing search integration
- Build a client portal

---

## Support

For help with this template:
- Check OpenClaw docs
- Join the OpenClaw community
- Refer to the README in the package

---

*This template is a starting point. Customize heavily for your specific needs and market.*