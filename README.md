# CY Hsieh

Trading systems engineer, Rust and Python. I build and run the infrastructure a
systematic strategy needs: exchange connectivity, market-data pipelines,
backtest-to-live parity, and the live node itself. MSc in Mathematics, National
Chengchi University, finishing in 2027. Based in Taipei; open to Amsterdam,
London and remote roles.

## Open source

- **[NautilusTrader](https://github.com/nautechsystems/nautilus_trader)** —
  [13 merged pull requests](https://github.com/nautechsystems/nautilus_trader/pulls?q=is%3Apr+is%3Amerged+author%3AMartingale42)
  to the open-source trading engine: exchange connectivity (Bybit) and
  portfolio risk statistics.
- **[sinopac-nt-community](https://github.com/Martingale42/sinopac-nt-community)** —
  NautilusTrader adapter for the Taiwan stock and futures markets, in Rust
  with Python bindings; published on PyPI and crates.io.
- **[nt-parquet-writer-bench](https://github.com/Martingale42/nt-parquet-writer-bench)** —
  benchmark of Parquet storage settings for market data; found a default that
  wastes space on every price column.
- **[small-vLLM](https://github.com/Yu-TingLee/small-vLLM)** — a C++/CUDA LLM
  inference engine, where I contribute alongside the author.
- **[nautilus-dev](https://github.com/Martingale42/nautilus-dev)** — AI agent
  skills for developing on NautilusTrader.

## Private work

Most of my commits are in private repositories:

- A **live trading node** on Polymarket, on NautilusTrader 2.0 on AWS, since
  October 2026.
- A **research lab** where NautilusTrader v2 carries all backtest and trading
  logic: Bybit and Binance perpetual L2 replays, Polymarket up/down markets,
  US ETF and TAIFEX bars.
- A **multi-strategy live node fleet** on NautilusTrader v2's Rust core,
  deployed with Docker.
- **Trading-host infrastructure as code** on AWS, with a latency harness.

## Competitions and research

- WorldQuant International Quant Championship 2026: top 1% of 150k+ teams;
  offered a Research Consultant role.
- MSc thesis: entropy of weighted independent-set models on Hanoi graphs
  (combinatorics and probability), with computer-checked results regenerated
  from one configuration.

## How I work

I run AI coding agents the way a lead runs a team: I write the spec, they
write the code, and nothing ships without review.

- **Spec first.** Every change starts as a design document, is cut into
  tickets with explicit dependencies, and is implemented by agents in isolated
  worktrees. Nothing merges without a three-axis review (spec, standards,
  attack) and green CI. Several of the repositories above went from empty to
  production this way in weeks.
- **My own toolkit.** I maintain a set of 25 agent skills that cover the whole
  loop, from interviewing the owner to landing the branch, with a measurement
  harness that checks each skill changes agent behaviour the way it claims.
  Public release is in progress.
- **My own stack.** The agents run on a self-hosted inference stack (vLLM and
  llama.cpp on my own GPUs) as well as hosted models, so I know what the
  models cost, where they fail, and how to route around it.
- **Documents are the memory.** Every repository carries a status page,
  decision records and a glossary, so a person or an agent can pick the work
  up cold.

[LinkedIn](https://www.linkedin.com/in/cy-hsieh)
