# Free LLM APIs — Grouped by Rate-Limit Reset Cadence

<p align="center">
  <img alt="Provider Logos" src="https://github.com/open-free-llm-api/awesome-freellm-apis/raw/main/assets/provider-logos-marquee.svg" width="100%" />
</p>

> **Credit & thanks:** All provider data, rate limits, and API key links sourced from [**open-free-llm-api/awesome-freellm-apis**](https://github.com/open-free-llm-api/awesome-freellm-apis) — an excellent, actively-maintained directory of free LLM APIs, refreshed daily. Go star the repo and check out [freellm.net](https://freellm.net) for the full live dataset, playground, and config generator. This doc just re-slices their data by reset cadence for quick reference.

Source: [open-free-llm-api/awesome-freellm-apis](https://github.com/open-free-llm-api/awesome-freellm-apis) (data as of 2026-08-18)

These are providers whose free tier is **rate/quota-based with automatic reset** — not a one-time credit balance that runs out permanently. Once you hit the cap, it refills on its own clock, no payment needed.

**Excluded** (fixed credit balance, spent down, not cleanly auto-refreshing): xAI, Grok (xAI), OpenRouter's paid $10-topup tier, Cline.

> **Correction:** Hugging Face was previously listed as excluded. Its free-tier $0.10/month Inference Provider credit does in fact auto-renew every month (confirmed via HF's official pricing docs) — it just hard-stops for the rest of the month once spent, since free users don't get pay-as-you-go overflow like PRO/Enterprise. It's now listed under **Monthly**.

---

## Per-minute (fastest refill)

| Provider | Free Models | Limit | Get Key |
|---|---|---|---|
| NVIDIA NIM | 125 | Up to 40 RPM | [→](https://build.nvidia.com/settings/api-keys) |
| LLM7.io | 16 | 30 RPM (120 w/ token) | [→](https://token.llm7.io) |
| OVHcloud AI Endpoints | 14 | 2 RPM (anonymous) | [→](https://www.ovhcloud.com/en/public-cloud/ai-endpoints/catalog/) |
| Cohere | 12 | 20 RPM | [→](https://dashboard.cohere.com/api-keys) |
| Mistral AI | 12 | ~1 RPS, 500K TPM | [→](https://console.mistral.ai/api-keys) |
| Agnes AI | 5 | 30 RPM | [→](https://platform.agnes-ai.com/settings/apiKeys) |
| SiliconFlow | 3 | 30 RPM, 60K TPM | [→](https://cloud.siliconflow.cn/account/ak) |
| AI21 Labs | 2 | 200 RPM, 10 RPS | [→](https://studio.ai21.com/account/api-key) |

## Per-minute + per-day combo

| Provider | Free Models | Limit | Get Key |
|---|---|---|---|
| Google Gemini | 17 | 15–30 RPM, 1,500 RPD | [→](https://aistudio.google.com/app/apikey) |
| Groq | 12 | 30 RPM, 14,400 RPD | [→](https://console.groq.com/keys) |
| Cerebras | 8 | 5 RPM, 30K TPM, 1M TPD | [→](https://cloud.cerebras.ai/) |
| Aion Labs | 7 | 15 RPM, 20K TPD | [→](https://www.aionlabs.ai) |
| SambaNova | 4 | 20 RPM, 20 RPD, 200K TPD | [→](https://cloud.sambanova.ai/apis) |

## Daily

| Provider | Free Models | Limit | Get Key |
|---|---|---|---|
| Cloudflare Workers AI | 39 | 10K Neurons/day, resets 00:00 UTC | [→](https://dash.cloudflare.com/profile/api-tokens) |
| ModelScope | 55 | 2,000 RPD (model-dependent) | [→](https://modelscope.cn/my/myaccesstoken) |
| GitHub Models | 16 | See provider (daily windows) | [→](https://github.com/marketplace/models) |
| OpenRouter (free models) | 26 | 50 RPD/model, no-topup | [→](https://openrouter.ai/workspaces/default/keys) |

## 5-hour / 7-day dual clock

| Provider | Free Models | Limit | Get Key |
|---|---|---|---|
| Ollama Cloud | 13 | Session (5h) + weekly (7d) reset | [→](https://ollama.com/settings/keys) |

## Hourly

| Provider | Free Models | Limit | Get Key |
|---|---|---|---|
| Kilo Code | 12 | ~200 req/hr | [→](https://kilo.ai) |

## Monthly

| Provider | Free Models | Limit | Get Key |
|---|---|---|---|
| Hugging Face | 7 | $0.10 in Inference Provider credits, auto-renews monthly — hard stop when exhausted (no PAYG on free tier) | [→](https://huggingface.co/settings/tokens) |

## Dynamic / fair-use (no fixed number, never depletes)

| Provider | Free Models | Limit | Get Key |
|---|---|---|---|
| Z AI (Zhipu AI) | 4 | 1 concurrent request | [→](https://open.bigmodel.cn/usercenter/apikeys) |
| DeepSeek | 2 | Dynamic (server-load based) | [→](https://platform.deepseek.com/api_keys) |
| Nscale | 2 | Fair-use | [→](https://console.nscale.com/) |
| Alibaba Cloud Model Studio | 5 | Tiered by region | [→](https://bailian.console.alibabacloud.com/?apiKey=1) |
| Nebius | 1 | Tier-based | [→](https://studio.nebius.com/settings/api-keys) |
| OpenCode Zen | 11 | See provider | [→](https://opencode.ai/auth) |
| Glhf.chat | 2 | Unlimited for free models | [→](https://glhf.chat/) |
| Chutes.ai | 2 | Community-powered, no hard cap (unconfirmed clean reset) | [→](https://chutes.ai/) |

---

> ## Excluded — Credit/Balance Based (Not Auto-Refreshing)
>
> | Provider | Why excluded |
> |---|---|
> | xAI | Credit-based |
> | Grok (xAI) | $25/month free credits, spent down |
> | OpenRouter (paid tier) | One-time $10 topup unlocks 1K RPD, not a recurring free grant |
> | Cline | Registration-gated, reset mechanics unconfirmed |
