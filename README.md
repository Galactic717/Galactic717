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
| [skillrot](https://github.com/Galactic717/skillrot) | Shows how much of an AI agent's context its skill library takes up | Weekly CI audit of 5 public libraries |
| [VaultDrop](https://github.com/Galactic717/VaultDrop) | Offline Windows backups that read back and verify every file | Installer and CLI in [v0.2.0](https://github.com/Galactic717/VaultDrop/releases/tag/v0.2.0) |
| [RoadForge](https://github.com/Galactic717/roadforge) | Self-driving demo on real OpenStreetMap roads, in the browser | [Live demo](https://galactic717.github.io/roadforge/); 0 collisions in 20 benchmark runs |

Right now I'm training my own 158M-parameter language model from scratch on Ukrainian, English and code.
That repo stays private until a checkpoint is worth sharing.

## How I work

I write code together with AI coding agents (Claude Code, Codex) and hold it to the same bar as anything else:
tests, CI, and a benchmark before I call a change an improvement. The numbers above come from those tests and
benchmarks, not from estimates.
