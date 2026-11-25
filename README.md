# 🤖 Luca Autonomous Web & Market Intelligence API (x402 Enabled)

Pay-per-request autonomous web scraping, multi-source fact-checking, and real-time crypto/tech market intelligence API powered by **ZeroClaw** and **x402 (Base Mainnet USDC)**.

No API keys, no subscriptions, no rate-limit signups—just standard HTTP `402 Payment Required` machine-to-machine micropayments.

## 🌐 Base Endpoint
`https://x402.my-cdn.net`

## 💳 Payment Details
- **Protocol:** x402 (v2)
- **Network:** Base Mainnet (`eip155:8453`)
- **Currency:** USDC (`0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913`)

## 🛠️ Available Endpoints

| Method | Endpoint | Price (USDC) | Description |
| :--- | :--- | :--- | :--- |
| `GET` | `/health` | Free | Check service status and active endpoints |
| `POST` | `/scrape` | **$0.03** | Live Web Scraper & Clean Markdown/JSON Extractor (with automatic search fallback) |
| `POST` | `/research` | **$0.05** | Deep Web Research & Multi-Source Fact-Check Synthesizer |
| `POST` | `/intel` | **$0.08** | Real-Time Crypto & Tech Market Intelligence Brief (Structured JSON) |
| `POST` | `/run` | **$0.05** | All-in-One Autonomous Web Research & Data Extractor |

## 🚀 Quick Example (cURL)

```bash
curl -X POST https://x402.my-cdn.net/scrape \
  -H "Content-Type: application/json" \
  -d '{"prompt": "Extract the main headlines and key data from https://example.com"}'
```

*First request returns `HTTP 402 Payment Required` with payment instructions in the `payment-required` header. Complete payment via any x402-compatible client (`x402-fetch`, `x402-httpx`, Coinbase AgentKit, etc.) to receive the synthesized result.*
