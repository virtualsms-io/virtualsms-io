# VirtualSMS

**Real carrier SIMs. Matching-country IPs. Private browser. One balance.**

VirtualSMS is an account verification platform for individuals, businesses, developers, and AI agents. It combines one-time SMS verification, dedicated number rentals, matching-country proxies, and private cloud browser sessions behind one API, one MCP server, and one prepaid balance.

Numbers are carrier-issued mobile numbers, backed by real physical SIM cards, not VoIP. Telegram, WhatsApp, Google, and 2500+ other services run a carrier lookup before they send a code, and VoIP numbers fail it more often than a real SIM does. That is a 95%+ success rate across 2500+ services in 145+ countries.

[Get a number](https://virtualsms.io/verifications) &nbsp;·&nbsp; [Browse services and prices](https://virtualsms.io) &nbsp;·&nbsp; [Read the docs](https://virtualsms.io/docs)

---

## Skip the retry loop

VoIP numbers get rejected. Real SIMs pass. That is the whole product.

- **See the price before you sign up.** Real prices, live stock, no surprises at checkout.
- **Codes arrive in seconds.** No code within 20 minutes? Your balance is auto-refunded, so you never pay for a failed verification.
- **Keep your real number private.** Numbers run on real operators like Vodafone, O2, and T-Mobile, so signups land on a genuine carrier, not a burner VoIP line.
- **Prove it yourself.** Check any number's line type free with the [number checker](https://virtualsms.io/tools/number-checker). VoIP shows up as VoIP. Ours does not.

---

## Four products, one balance

Most providers solve one piece of the verification workflow. VirtualSMS gives you all four behind one API and one prepaid balance, so you use only the pieces you need or combine them into a single flow.

| Product | What you get | From |
|---|---|---|
| **Verifications** | One-time SMS codes for 2500+ services on real carrier SIMs. Works where VoIP does not. | $0.05 / code |
| **Rentals** | Keep a number by the day, 1 to 30 days. Full Access or Platform tier, refundable within 20 minutes. | $0.25 / day |
| **Proxies** | Matching-country proxies across 190+ countries, wider coverage than the numbers themselves. | $1.10 / GB |
| **Cloud Browser** *(beta)* | Start a country-matched browser and drive the signup yourself in a live viewer. | Self-serve beta |

Your number, your IP, and your browser tell the same story. One country, one balance, no stitching three vendors together.

---

## For developers and AI agents

**Infrastructure for AI agents that need real-world phone verification.** One hosted MCP server exposes the whole platform as 40 tools, so any MCP client can buy a number, wait for the code, rent a number, and buy or rotate a proxy with no wrapper code to write.

### Hosted MCP server (recommended)

Point any streamable-http MCP client at the hosted endpoint and pass your API key. Always the latest version, zero install.

```json
{
  "mcpServers": {
    "virtualsms": {
      "url": "https://mcp.virtualsms.io/mcp",
      "headers": { "x-api-key": "your-api-key" }
    }
  }
}
```

### Or run it locally over stdio

```bash
npx virtualsms-mcp
```

```json
{
  "mcpServers": {
    "virtualsms": {
      "command": "npx",
      "args": ["virtualsms-mcp"],
      "env": { "VIRTUALSMS_API_KEY": "your-api-key" }
    }
  }
}
```

The 40 tools cover verification and account (18), rentals (9), proxies (10), and utilities including the free number checker and cloud-browser session start (3). Full setup for Claude, Cursor, Windsurf, and every major client lives at [virtualsms.io/mcp](https://virtualsms.io/mcp).

**Example prompts**

```
Verify a Telegram account using the cheapest available country
Buy a UK number for WhatsApp verification
Rent a number for 7 days locked to WhatsApp
Find a residential proxy in Germany and rotate it for a new IP
Check my balance and list active orders
```

---

## Official SDKs

The same REST API, idiomatic in your language. All published and versioned.

| Language | Package | Install | Repo |
|---|---|---|---|
| Node.js | `virtualsms-sdk` | `npm install virtualsms-sdk` | [node-sdk](https://github.com/virtualsms-io/node-sdk) |
| Python | `virtualsms` | `pip install virtualsms` | [python-sdk](https://github.com/virtualsms-io/python-sdk) |
| PHP | `virtualsms/sdk` | `composer require virtualsms/sdk` | [virtualsms-php-sdk](https://github.com/virtualsms-io/virtualsms-php-sdk) |
| Ruby | `virtualsms-sdk` | `gem install virtualsms-sdk` | [ruby-sdk](https://github.com/virtualsms-io/ruby-sdk) |
| .NET | `VirtualSMS` | `dotnet add package VirtualSMS` | [dotnet-sdk](https://github.com/virtualsms-io/dotnet-sdk) |
| Rust | `virtualsms` | `cargo add virtualsms` | [rust-sdk](https://github.com/virtualsms-io/rust-sdk) |
| Go | `github.com/virtualsms-io/go-sdk/v2` | `go get github.com/virtualsms-io/go-sdk/v2@v2.0.0` | [go-sdk](https://github.com/virtualsms-io/go-sdk) |
| Java | `io.virtualsms:sdk` | `implementation("io.virtualsms:sdk:2.0.0")` (Maven Central) | [java-sdk](https://github.com/virtualsms-io/java-sdk) |
| Swift | `swift-sdk` (SPM) | `.package(url: "https://github.com/virtualsms-io/swift-sdk.git", from: "2.0.0")` | [swift-sdk](https://github.com/virtualsms-io/swift-sdk) |

No code? Drive the same API from [n8n](https://github.com/virtualsms-io/n8n-nodes-virtualsms) (`npm i n8n-nodes-virtualsms`), or drop in the ready-made [Claude skill](https://github.com/virtualsms-io/claude-skill-sms-verification) and [Cursor rules](https://github.com/virtualsms-io/cursor-rules-sms-verification). Zapier and Activepieces integrations are in development.

---

## Links

- 🌐 Website: [virtualsms.io](https://virtualsms.io)
- 🤖 MCP server: [virtualsms.io/mcp](https://virtualsms.io/mcp)
- 📖 API docs: [virtualsms.io/docs](https://virtualsms.io/docs)
- 📝 Blog: [virtualsms.io/blog](https://virtualsms.io/blog)
- 🐦 X: [@VirtualSMSio](https://x.com/VirtualSMSio)
- 💬 Telegram: [@VirtualSMS_io](https://t.me/VirtualSMS_io)
- 📺 YouTube: [@VirtualSMSio](https://www.youtube.com/@VirtualSMSio)
- 🧑‍💻 dev.to: [@virtualsms](https://dev.to/virtualsms)

---

## Explore with AI

[Ask ChatGPT](https://chatgpt.com/?prompt=Summarize+VirtualSMS+at+https%3A%2F%2Fvirtualsms.io) &nbsp;·&nbsp; [Ask Claude](https://claude.ai/new?q=Tell+me+about+VirtualSMS+at+https%3A%2F%2Fvirtualsms.io) &nbsp;·&nbsp; [Ask Perplexity](https://www.perplexity.ai/search/?q=VirtualSMS+account+verification+platform) &nbsp;·&nbsp; [Ask Gemini](https://gemini.google.com/app?q=Tell+me+about+VirtualSMS+at+https%3A%2F%2Fvirtualsms.io) &nbsp;·&nbsp; [Ask Grok](https://grok.com/?q=VirtualSMS+account+verification+for+humans+and+AI+agents)

---

**Real carrier SIMs, matching-country proxies, and a private browser behind one API, one MCP server, and one prepaid balance. Built for individuals, businesses, developers, and AI agents.**
