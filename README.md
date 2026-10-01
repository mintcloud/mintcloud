## Theo Gonella

Product leader — AI systems, crypto, DeFi. Barcelona.

Head of Product, DeFi at [Kiln](https://www.kiln.fi) through April 2026, where I launched OmniVault and Railnet with CoinShares and Monarq as institutional launch partners. Before that, Director of Product at [0x / matcha.xyz](https://0x.org) — open-source protocol to a 600-customer API business. Before that, Ads at Facebook. Aerospace engineer by training.

### What I run

A multi-model LLM agent fleet on my own hardware, dispatched over Telegram by voice and text. Since February 2026:

- **~3,500 briefs** dispatched · **8,000+ documents** produced · **5.1B tokens**
- **12 models**, tiered. 63% of runs mix tiers in a single pass; the cheap tier carries that 63% for **3% of total spend**
- **$0.79 median brief.** Instrumented to the unit cost of a single answer — which is how I found that cache reads are 94.3% of input tokens at 93.8× amplification, and that the expensive part of an agent is not retrieval but *retention*

It writes its own memory — an append-only journal compiled into ~220 entity pages, loaded at every dispatch — and runs a nightly reflection over the day's work, then weekly and monthly consolidations.

### What I build with it

- **[expatrimony.com](https://www.expatrimony.com)** — untangles state pensions across borders. Production LLM extraction over arbitrary PDFs: structured outputs, dual provider (metered API + self-hosted fallback), and an eval harness that grades extracted numbers against a tolerance on a weekly cron, deliberately kept out of PR CI because a probabilistic extractor has no business gating a merge.
- **[loopclub](https://loopclub.xyz)** — a 16×4 drum machine that lives entirely onchain, on MegaETH. Ships with an MCP server, so you can describe a beat to Claude and get back a playable link.
- **[shillscore](https://github.com/mintcloud/shillscore)** — signal-scoring for a noisy timeline.

<!-- Uncomment as they go public:
### Published

- **[llm-extraction-eval](https://github.com/mintcloud/llm-extraction-eval)** — the eval harness above, standalone. Tolerance-based grading, dual provider, scheduled rather than per-push.
- **[agent-fleet-economics](https://github.com/mintcloud/agent-fleet-economics)** — measure where the money actually goes in an agent fleet. Runs against your own Claude Code history.
-->

[theogonella.com](https://theogonella.com) · [x.com/theogonella](https://x.com/theogonella) · [linkedin](https://linkedin.com/in/theogonella)
