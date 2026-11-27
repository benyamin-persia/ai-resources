# MeMo — Memory as a Model

Shared in [CrazyShyyt's X post](https://x.com/CrazyShyyt/status/2125859848965534161), which describes the [MeMo paper](https://arxiv.org/abs/2605.15156) and its [implementation](https://github.com/arunv3rma/MeMo). MeMo trains a separate memory model on synthesized question/answer reflections from a document corpus. At inference, a frozen executive LLM queries that memory model through a multi-turn protocol; it does not use a conventional retrieval index for the tested setup.

- Paper: [MeMo: Memory as a Model (arXiv:2605.15156)](https://arxiv.org/abs/2605.15156)
- Code: [arunv3rma/MeMo](https://github.com/arunv3rma/MeMo)
- Your individual fork: [benyamin-persia/MeMo](https://github.com/benyamin-persia/MeMo) (verified parent: `arunv3rma/MeMo`)
- Code license: MIT, according to the implementation repository.

## What the paper reports

On NarrativeQA, the paper reports 53.58% accuracy for MeMo with Gemini-3-Flash versus 23.21% for the HippoRAG2 baseline; with Qwen2.5-32B-Instruct, the corresponding scores are 26.85% and 21.39%. The evaluation covers three benchmarks and compares against specific retrieval and memory baselines; these results do not establish that RAG is generally obsolete. The reported method also requires per-corpus data synthesis and memory-model fine-tuning. The paper's limitations include training cost, evaluation scope, and how memory-model capacity scales with corpus size.

The 53.58% Gemini result is a single reported run, while the Qwen result is averaged across three runs. Review the paper and repository for experimental setup and resource requirements before drawing broader conclusions.
