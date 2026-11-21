# Hlib Stepanov

Second-year software engineering student at Taras Shevchenko National University of Kyiv. I work on applied AI:
agents that act on a computer under the user's control, search over private documents, and benchmarks that turn
"it works" into a number.

Open to junior AI engineer roles and internships, remote. [LinkedIn](https://www.linkedin.com/in/hlib-stepanov-3536a437b) · stepanovgleb10@gmail.com

## Projects

| Project | What it is | Measured |
|---|---|---|
| [Halo Bot](https://github.com/Galactic717/halo-bot) | Desktop app where AI assistants do real work on your PC, each in its own Windows sandbox, behind an approval gate and an audit log | On an 11-task benchmark a local 4B model went from 7 to 10 solved tasks ([PR #14](https://github.com/Galactic717/halo-bot/pull/14)) |
| [Glossa](https://github.com/Galactic717/glossa) | Ask your documents a question and get the answer with the page it came from. 35 languages, runs offline | Retrieval pipeline in about 300 lines, no LangChain |
| [vybir](https://github.com/Galactic717/vybir) | Runs an AI decision model on ordinary PCs and hands the cases it isn't sure about to a person | Per-class calibration cut spam that got through from 23.8% to 3.5%; 183 tests |
| [VARTA](https://github.com/Galactic717/varta) | Live air-threat map of Ukraine with a Q&A agent that computes distances and ETA in code instead of letting the model invent them | Intent bake-off on 436 hand-labelled questions: mmBERT-small 89.7% vs GPT-2 at chance (8%); release v2.0.0 |
| [Copilot](https://github.com/Galactic717/copilot-rust) | Real-time interview and meeting assistant that runs on your PC: local speech recognition, answers built only from your CV, no account | One ~190 MB exe, interface in 12 languages, speech in 47; release v1.0.0 |
| [so-trust](https://github.com/Galactic717/so-trust) | Rates whether a Stack Overflow answer still works for the versions your project runs: STALE / CHECK / OK | Measured SO decay: 105,743 new questions/month in Oct 2022, 966 in Sep 2026; release v0.3.0 |
| [Telemetria](https://github.com/Galactic717/telemetria) | Real-time PC hardware telemetry, wall-power analysis and GPU rental/mining profitability as a Rust CLI/TUI | NVML sampling in 300–1200 µs; Rust CI |
| [skillrot](https://github.com/Galactic717/skillrot) | Shows how much of an AI agent's context its skill library takes up | Weekly CI audit of 5 public libraries |
| [VaultDrop](https://github.com/Galactic717/VaultDrop) | Offline Windows backups that read back and verify every file | Installer and CLI in [v0.2.0](https://github.com/Galactic717/VaultDrop/releases/tag/v0.2.0) |

Also public: [pcsleuth](https://github.com/Galactic717/pcsleuth) (plain-language answers from the logs Windows
already keeps; pre-alpha), [skillsmith](https://github.com/Galactic717/skillsmith) (Claude Code plugin that turns
a product idea into a verified build), [agent-skills-kit](https://github.com/Galactic717/agent-skills-kit)
(open SKILL.md collection with a validator), [log3-replication](https://github.com/Galactic717/log3-replication)
(protected event-log replication, KNU course project).

## How I work

I write code together with AI coding agents (Claude Code, Codex) and hold it to the same bar as anything else:
tests, CI, and a benchmark before I call a change an improvement. The numbers above come from those tests and
benchmarks, not from estimates.
