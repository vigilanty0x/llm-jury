# LLM Jury

> [!IMPORTANT]
> Canonical development has been consolidated into [`vigilanty0x/promptops`](https://github.com/vigilanty0x/promptops), under [`packages/llm-jury`](https://github.com/vigilanty0x/promptops/tree/main/packages/llm-jury). This repository remains available to preserve its source history and compatibility reference. The imported `0.1.0` package keeps the `llm-jury` distribution and CLI names. This notice does not claim a package-index transfer or publication.

Offline rubric jury aggregation with disagreement evidence.

Offline Python 3.11+ MVP with zero runtime dependencies, deterministic JSON evidence, bounded inputs, a CLI, synthetic tests, and fail-visible errors.

## Usage

```bash
python -m llm_jury.cli input.json
python -m unittest discover -s tests -v
python scripts/check.py
```

Input is a JSON object matching the public `run(data)` API in `llm_jury.core`. With no path, the CLI reads stdin.

Apache License 2.0.

