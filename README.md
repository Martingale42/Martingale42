# CY Hsieh

Trading systems engineer, Rust and Python. I build and run the infrastructure a
systematic strategy needs: exchange connectivity, market-data pipelines,
backtest-to-live parity, and the live node itself. MSc in Mathematics, National
Chengchi University, finishing in 2027. Based in Taipei; open to Amsterdam,
London and remote roles.

## Open source

- **[NautilusTrader](https://github.com/nautechsystems/nautilus_trader)** —
  [13 merged pull requests](https://github.com/nautechsystems/nautilus_trader/pulls?q=is%3Apr+is%3Amerged+author%3AMartingale42)
  since mid-2026. Bybit adapter: public liquidation custom data, WebSocket
  subscription state on reconnect, a non-terminating cursor in pagination.
  Portfolio statistics: VaR, Expected Shortfall, Omega ratio, tail ratio,
  skewness and kurtosis, plus rolling-window fixes in several indicators.
- **[sinopac-nt-community](https://github.com/Martingale42/sinopac-nt-community)** —
  community NautilusTrader adapter for SinoPac (Taiwan TWSE, TPEX and TAIFEX).
  Rust core with Python bindings through PyO3, released to
  [PyPI](https://pypi.org/project/sinopac-nt-community/) and
  [crates.io](https://crates.io/crates/sinopac-nt-community) from CI. A
  redesign is in progress. Its gateway process is
  [shioaji-server](https://github.com/Martingale42/shioaji-server) (archived).
- **[nt-parquet-writer-bench](https://github.com/Martingale42/nt-parquet-writer-bench)** —
  measures how Parquet writer settings change NautilusTrader catalog size and
  read cost on real Tardis data, verified row for row. It found that parquet-rs
  never dictionary-encodes decimal columns under the default writer version.
- **[small-vLLM](https://github.com/Yu-TingLee/small-vLLM)** — a C++/CUDA LLM
  inference engine on LibTorch (paged KV cache, continuous batching, custom
  attention kernels). I contribute alongside the author: safetensors weight
  loading, ops dispatch and RMSNorm, build and CI tooling.
- **[nautilus-dev](https://github.com/Martingale42/nautilus-dev)** — agent
  skills for building with and on NautilusTrader, in Python and Rust.

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

Design document first, then tickets, implementation in isolated worktrees, a
three-axis review before merge, and CI as the gate. Much of it is agent-assisted,
with a skill set I maintain for that purpose.

[LinkedIn](https://www.linkedin.com/in/cy-hsieh)
