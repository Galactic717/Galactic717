# Hlib Stepanov

Second-year software engineering student at Taras Shevchenko National University of Kyiv. I work across the LLM
lifecycle: fine-tuning and evaluating small models, serving them, and building agents that act under the user's
control, with a benchmark behind every claim.

Open to junior AI engineer roles and internships, in Kyiv or remote. [LinkedIn](https://www.linkedin.com/in/hlib-stepanov-3536a437b) · stepanovgleb10@gmail.com

## LLM engineering

| Project | What it is | Measured |
|---|---|---|
| [Verifine SLM](https://github.com/Galactic717/verifine-slm) | Local structured extraction for Ukrainian and English documents: QLoRA SFT, then GRPO with verifiable rewards; returns `null` instead of guessing | Qwen3-4B on 300 held-out synthetic documents: field macro-F1 0.947 → 0.985, all fields correct 77.7% → 93.0%, schema validity 100% |
| [vllm-ops-kit](https://github.com/Galactic717/vllm-ops-kit) | LLM serving from Windows llama.cpp to Kubernetes and vLLM, with Helm, Terraform, Prometheus/Grafana and k6 checked in CI on a live kind cluster | Helm install to ready in 20.5 s; 30 req/s at a 3× spike with 0% HTTP errors (CPU fixture) |
| [Verstak Agent](https://github.com/Galactic717/verstak-agent) | Durable business workflows on LangGraph and PostgreSQL: a triage agent proposes, an evidence agent checks the source, a person approves; MCP control plane | Qwen3-4B Q4_K_M: tool-call F1 0.915, grounded field accuracy 96.7%; 79 tests at 87% line coverage |
| [LLM FinOps Warehouse](https://github.com/Galactic717/llm-finops-dw) | Lakehouse for LLM costs, inference telemetry and routing A/B tests: dbt, Airflow, Delta Lake, PostgreSQL, Power BI | PostgreSQL query 1,122 ms → 2.11 ms on one million rows; simulated hybrid routing cut mean modeled cost by 72.7% |
| [VARTA](https://github.com/Galactic717/varta) | Live air-threat map of Ukraine with a Q&A agent that computes distances and ETA in code instead of letting the model invent them | Intent bake-off on 436 hand-labelled questions: mmBERT-small 89.7% vs GPT-2 at chance (8%); release v2.0.0 |
| [Halo Bot](https://github.com/Galactic717/halo-bot) | Desktop app where AI assistants do real work on your PC, each in its own Windows sandbox, behind an approval gate and an audit log | On an 11-task benchmark a local 4B model went from 7 to 10 solved tasks ([PR #14](https://github.com/Galactic717/halo-bot/pull/14)) |
| [Glossa](https://github.com/Galactic717/glossa) | Ask your documents a question and get the answer with the page it came from. 35 languages, runs offline | Retrieval pipeline in about 300 lines, no LangChain |

## Other tools

| Project | What it is | Measured |
|---|---|---|
| [vybir](https://github.com/Galactic717/vybir) | Runs an AI decision model on ordinary PCs and hands the cases it isn't sure about to a person | Per-class calibration cut spam that got through from 23.8% to 3.5%; 183 tests |
| [Copilot](https://github.com/Galactic717/copilot-rust) | Real-time interview and meeting assistant that runs on your PC: local speech recognition, answers built only from your CV, no account | One ~190 MB exe, interface in 12 languages, speech in 47; release v1.0.0 |
| [so-trust](https://github.com/Galactic717/so-trust) | Rates whether a Stack Overflow answer still works for the versions your project runs: STALE / CHECK / OK | Measured SO decay: 105,743 new questions/month in Oct 2022, 966 in Sep 2026; release v0.3.0 |
| [Telemetria](https://github.com/Galactic717/telemetria) | Real-time PC hardware telemetry, wall-power analysis and GPU rental/mining profitability as a Rust CLI/TUI | NVML sampling in 300–1200 µs; Rust CI |

Also public: [skillrot](https://github.com/Galactic717/skillrot) (how much of an agent's context its skill library
takes up), [VaultDrop](https://github.com/Galactic717/VaultDrop) (offline Windows backups that verify every file),
[pcsleuth](https://github.com/Galactic717/pcsleuth) (plain-language answers from the logs Windows already keeps;
pre-alpha), [skillsmith](https://github.com/Galactic717/skillsmith) (Claude Code plugin that turns a product idea
into a verified build), [agent-skills-kit](https://github.com/Galactic717/agent-skills-kit) (open SKILL.md
collection with a validator), [log3-replication](https://github.com/Galactic717/log3-replication) (protected
event-log replication, KNU course project).

## How I work

I write code together with AI coding agents (Claude Code, Codex) and hold it to the same bar as anything else:
tests, CI, and a benchmark before I call a change an improvement. The numbers above come from those tests and
benchmarks, not from estimates.
