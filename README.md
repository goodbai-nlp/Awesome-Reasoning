# Awesome Reasoning

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <img src="https://img.shields.io/badge/Reasoning-Papers-blue" alt="Reasoning Papers">
<a href="https://github.com/goodbai-nlp/Awesome-Reasoning/stargazers">
  <img src="https://badgen.net/github/stars/goodbai-nlp/Awesome-Reasoning" alt="GitHub stars"></a>
<a href="https://github.com/goodbai-nlp/Awesome-Reasoning/network/members">
  <img src="https://badgen.net/github/forks/goodbai-nlp/Awesome-Reasoning" alt="GitHub forks"></a>
</p>

Awesome Reasoning is a curated collection of papers, benchmarks, datasets, codebases, and surveys related to reasoning in large language models, multimodal models, and agentic systems.

If you find this repository helpful, please consider giving us a star.

The collection is organized by major reasoning directions, with cross-cutting type tags such as `survey`, `method`, `benchmark`, `dataset`, `evaluation`, `analysis`, and `system`.

# Bookmarks

- [🏷️ Paper Type Tags](#paper-type-tags)
- [🧭 Categories](#categories)
- [🤝 Contribution Guide](#contribution-guide)
- [🌟 Contributors](#contributors)

<a id="paper-type-tags"></a>

## 🏷️ Paper Type Tags

| Type | Meaning |
| ---- | ------- |
| `survey` | Surveys, roadmaps, taxonomies, and overview papers |
| `method` | New algorithms, prompting strategies, search methods, or reasoning frameworks |
| `model` | Released reasoning models or model families |
| `training` | SFT, RL, distillation, reward modeling, or self-improvement recipes |
| `benchmark` | Evaluation suites, leaderboards, or test protocols |
| `dataset` | Training, evaluation, or synthetic data resources |
| `evaluation` | Empirical comparisons, audits, and capability measurements |
| `analysis` | Mechanistic, behavioral, scaling, or failure-mode analysis |
| `system` | Tooling, libraries, serving systems, and reproducible infrastructure |
| `application` | Domain-specific reasoning applications |

<a id="categories"></a>

## 🧭 Categories

| Category | Focus | Link |
| -------- | ----- | ---- |
| Learning-to-Reason | Training and post-training methods that improve general reasoning ability, including SFT, RL, verifiers, process rewards, and self-improvement. | [README](learning-to-reason/README.md) |
| Test-Time Scaling | Methods that spend more or better compute during inference, including sampling, search, verification, and refinement. | [README](test-time-scaling/README.md) |
| Efficient Reasoning | Methods that reduce reasoning cost, latency, token length, or memory while preserving reasoning quality. | [README](efficient-reasoning/README.md) |
| Structured / Symbolic / Verifiable Reasoning | Reasoning over math, logic, code, tables, graphs, databases, knowledge graphs, and other structured or checkable domains. | [README](structured-symbolic-reasoning/README.md) |
| Multimodal Reasoning | Reasoning across images, videos, audio, documents, charts, 3D scenes, GUI states, and embodied environments. | [README](multimodal-reasoning/README.md) |
| Agentic Reasoning | Planning, tool use, reflection, memory, multi-agent collaboration, and long-horizon interactive task solving. | [README](agentic-reasoning/README.md) |

<a id="contribution-guide"></a>

## 🤝 Contribution Guide

We welcome readers and community members to join us in keeping this repository up to date.

- Add each paper to the most relevant primary category.
- Use tags to capture secondary dimensions.
- Prefer official paper, code, project, dataset, and benchmark links.
- Keep notes short: one sentence is usually enough.
- If a paper introduces both a method and a benchmark, list it where the main contribution is stronger and tag the other type.

<a id="contributors"></a>

## 🌟 Contributors

Thanks to all contributors who help maintain and improve this repository.

<!-- ALL-CONTRIBUTORS-LIST:START -->
<a href="https://github.com/goodbai-nlp/Awesome-Reasoning/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=goodbai-nlp/Awesome-Reasoning" alt="Contributors">
</a>
<!-- ALL-CONTRIBUTORS-LIST:END -->
