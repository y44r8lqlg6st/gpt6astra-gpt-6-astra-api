# GPT-6 Astra API (gpt-6-astra / gpt6astra) — llm guide with published pricing

> **input $8; cached_input $0.8; cache_write $10** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-43b9f9)** · **[Get an API key](https://go.apimart.ai/k-657f84)**

Everything here refers to **gpt-6-astra** — also written **gpt6astra** or **gpt 6 astra**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `input` | $8 |
| `cached_input` | $0.8 |
| `cache_write` | $10 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $800 |
| 1,000 | $8,000 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"gpt-6-astra","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
