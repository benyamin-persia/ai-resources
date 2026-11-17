# Qwen3.8-27B with TensorFold and DFlash2

Shared in [Oluwaphilemon1's X post](https://x.com/Oluwaphilemon1/status/2122469810214744565), with a [demonstration video](https://x.com/pratikg/status/2117801754989592866/video/1).

The post describes running Qwen3.8-27B on a Mac mini with an M5 Pro and 64 GB unified memory, using TensorFold and DFlash2 speculative decoding. It reports 17 tokens/s without DFlash2, 56 tokens/s with it, and a peak of 91.90 tokens/s in a coding evaluation. It also reports 28.5 GiB peak memory and TensorFold 1.2.1/1.2.2 results, including 3.26x–3.35x chat speedups, 2.77x–2.94x on a 31K-token long-context test, and 5.4x–5.5x in coding.

These are claims from the post, not independently verified benchmarks. The post does not link a specific Qwen3.8-27B model checkpoint or benchmark harness, so exact reproducibility cannot be assessed from the post alone.

TensorFold is the GitHub project associated with the inference engine named in the post: [upstream repository](https://github.com/ashhart/TensorFold) · [your fork](https://github.com/benyamin-persia/TensorFold). DFlash2 is named as the speculative decoding method; no separate DFlash2 repository or model checkpoint is linked in the post.

Confirm the model build, quantization, TensorFold version, DFlash2 drafter, context length, and benchmark procedure against the [TensorFold project](https://github.com/ashhart/TensorFold) before trying to reproduce the reported figures.
