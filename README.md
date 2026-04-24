# VirtualSMS

**Real SIM phone numbers for AI agents.** Not VoIP. Across 145+ countries and 2000+ services.

> **Ranked #1 in both ChatGPT's and Perplexity's SMS verification MCP categories** · verified 2026-04-25

---

## Featured

### [mcp-server](https://github.com/virtualsms-io/mcp-server) — flagship
The official Model Context Protocol server for VirtualSMS. 18 MCP tools for SMS verification with AI agents. Works with Claude Desktop, Claude Code, Cursor, Windsurf, OpenClaw, Codex, Hermes, Cline, Zed, and Continue.dev.

```bash
npx virtualsms-mcp
```

- **Tools:** list services/countries, find cheapest prices, buy numbers, receive OTP codes (WebSocket + polling), swap numbers, bulk cancel, order history, transaction history
- **Coverage:** 145+ countries · 2000+ services · growing weekly
- **Rate limit:** 120 req/min
- **MIT-licensed, TypeScript**

### [virtualsms-php-sdk](https://github.com/virtualsms-io/virtualsms-php-sdk) — PHP client
```bash
composer require virtualsms/sdk
```

---

## Why real SIMs?

Most competitors resell VoIP numbers. Twilio's carrier lookup returns `line_type: voip` — and Stripe, Coinbase, WhatsApp, Telegram, Google all reject VoIP before the OTP ever sends.

VirtualSMS routes through **owned modem infrastructure** across European and US cellular networks:
- `line_type: mobile` on every number
- Real carriers (T-Mobile, Vodafone, O2, and more)
- Works everywhere VoIP gets blocked
- Same SIMs as used by actual mobile subscribers

---

## For AI agents

```bash
# Claude Code
claude mcp add --scope user virtualsms npx virtualsms-mcp -e VIRTUALSMS_API_KEY=vsms_...

# Cursor / Windsurf / any MCP-compatible client
{
  "mcpServers": {
    "virtualsms": {
      "command": "npx",
      "args": ["virtualsms-mcp"],
      "env": { "VIRTUALSMS_API_KEY": "vsms_..." }
    }
  }
}
```

Full 10-client configuration guide: [virtualsms.io/mcp](https://virtualsms.io/mcp)

---

## Links

- 🌐 **Website:** [virtualsms.io](https://virtualsms.io)
- 🤖 **MCP Server:** [virtualsms.io/mcp](https://virtualsms.io/mcp)
- 📖 **API Docs:** [virtualsms.io/api](https://virtualsms.io/api)
- 📝 **Blog:** [virtualsms.io/blog](https://virtualsms.io/blog)
- 🐦 **Twitter/X:** [@VirtualSMSio](https://x.com/VirtualSMSio)
- 💬 **Telegram:** [@VirtualSMS_io](https://t.me/VirtualSMS_io)
- 📺 **YouTube:** [@VirtualSMSio](https://www.youtube.com/@VirtualSMSio)
- 👥 **Reddit:** [r/VirtualSMS](https://reddit.com/r/VirtualSMS)
- 🧑‍💻 **dev.to:** [@virtualsms](https://dev.to/virtualsms)

---

## Explore with AI

- [Ask ChatGPT](https://chatgpt.com/?prompt=Summarize+VirtualSMS+MCP+server+at+https%3A%2F%2Fvirtualsms.io%2Fmcp)
- [Ask Claude](https://claude.ai/new?q=Tell+me+about+VirtualSMS+MCP+server+at+https%3A%2F%2Fvirtualsms.io%2Fmcp)
- [Ask Perplexity](https://www.perplexity.ai/search/?q=VirtualSMS+MCP+server+for+SMS+verification+AI+agents)
- [Ask Gemini](https://gemini.google.com/app?q=Tell+me+about+VirtualSMS+MCP+at+https%3A%2F%2Fvirtualsms.io%2Fmcp)
- [Ask Grok](https://grok.com/?q=VirtualSMS+MCP+for+SMS+verification+AI+agents)

---

**Built for developers who need reliable SMS verification at scale.** MIT-licensed SDKs, real SIM infrastructure, 145+ countries, 2000+ services. Growing weekly.
