# Dale Brain - Configuration Reference

## Email - LobsterMail
- **Email:** jakes-assist@lobstermail.ai
- **Account ID:** acct_gs6AFsW_Xt-DVzxg
- **Inbox ID:** ibx_8VMhGuQHdLR37s2J
- **Tier:** 0 (needs verification)
- **Token:** [SEE LOCAL CONFIG - DO NOT COMMIT]
- **Expires:** 2026-05-26

## Email - Other
- **AgentMail:** dale-assistant@agentmail.to
- **Zoho:** jakewedge.com (SPF, DKIM, DMARC configured)

## OpenClaw Config
- **Browser:** agent-browser (local Chrome)
- **Hunter.io API Key:** [IN OPENCLAW CONFIG]
- **GitHub Token:** [IN OPENCLAW CONFIG - ghp_am2...]
- **Model:** openrouter/minimax/minimax-m2.5

## Business Info
- **Jake:** 20+ years marketing & sales training
- **Goal:** Build multiple online businesses, starting with automation workflows

## Previous Inboxes (March 28, 2026 - EXPIRED/UNRECOVERABLE)
- jake-dale@lobstermail.ai
- dale@lobstermail.ai

**NOTE:** Without the old tokens (lm_sk_...), these cannot be recovered. Tokens were lost when session reset.

## How to Use

1. Read this file from GitHub on startup
2. Get actual credentials from local config: ~/.openclaw/workspace/MEMORY.md
3. For Lobstermail API calls, use token from local config

## API Example
curl -s -H "Authorization: Bearer [TOKEN]" -H "Content-Type: application/json" \
  -d '{"subject": "test", "body": {"text": "Hello"}}' \
  https://api.lobstermail.ai/v1/emails/send
