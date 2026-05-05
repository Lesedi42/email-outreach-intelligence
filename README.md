# x402 Web2 Nodes — 3 High-Yield API Services

Same setup as your Web3 nodes — Express.js + x402 payments + /stats endpoint.

## Nodes

| # | Name | Folder | Key Routes | Price Range |
|---|------|--------|------------|-------------|
| 8 | AI Prompt Optimizer      | `ai-prompt-optimizer/`       | POST /optimize/quick\|model\|bundle   | $0.03–$0.15 |
| 9 | SEO Intelligence         | `seo-intelligence/`          | POST /seo/meta\|keywords\|audit\|competitor | $0.02–$0.20 |
| 10| Email Outreach Intelligence | `email-outreach-intelligence/` | POST /outreach/email\|company\|icebreaker\|lead | $0.04–$0.25 |

## Deploy to Render

Same steps as your Web3 nodes:
1. Push each folder as its own GitHub repo
2. Render.com → New Web Service → connect repo
3. Render reads render.yaml automatically
4. Set env vars in Render dashboard (see below)
5. Copy live URL → paste into dashboard NODES config

## Environment Variables

### AI Prompt Optimizer
| Key | Required | Where to get |
|-----|----------|--------------|
| WALLET_ADDRESS | ✅ Yes | Your wallet |
| OPENAI_API_KEY | Optional | platform.openai.com — works without it using heuristics |

### SEO Intelligence
| Key | Required | Where to get |
|-----|----------|--------------|
| WALLET_ADDRESS | ✅ Yes | Your wallet |

### Email Outreach Intelligence
| Key | Required | Where to get |
|-----|----------|--------------|
| WALLET_ADDRESS | ✅ Yes | Your wallet |
| HUNTER_API_KEY | Optional | hunter.io — 25 free searches/month |
| OPENAI_API_KEY | Optional | platform.openai.com — for AI icebreakers |

## Revenue Potential

| Node | Est. Daily | Est. Monthly |
|------|-----------|--------------|
| AI Prompt Optimizer | $80–$200 | $2,400–$6,000 |
| SEO Intelligence | $100–$300 | $3,000–$9,000 |
| Email Outreach Intelligence | $150–$400 | $4,500–$12,000 |

## Works Without API Keys

All 3 nodes work out of the box with no external API keys:
- AI Prompt Optimizer → uses heuristic prompt rewriting
- SEO Intelligence → fetches and parses pages directly
- Email Outreach Intelligence → uses pattern-based email prediction

Add API keys later to upgrade to AI-powered / verified results.
