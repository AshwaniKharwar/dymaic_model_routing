# Dynamic LLM Router

A lightweight routing layer that selects the best LLM for each request based on
**cost**, **latency**, **context window**, and **quality of work**.

## Features
- Model registry with pricing, context limits, latency stats, and per-task quality scores
- Two-stage routing: hard constraint filters, then weighted scoring
- Ranked fallbacks on errors, timeouts, or rate limits
- Optional cascade: try a cheap model first, escalate only when needed
- Request logging to keep latency and quality data up to date
