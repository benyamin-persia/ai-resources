# Qwen3.8-27B on an RTX 3090: HyperQwen

Shared in [Oluwaphilemon1's X post](https://x.com/Oluwaphilemon1/status/2122531538973712512), which summarizes [TeksEdge's source post and demo](https://x.com/TeksEdge/status/2090595990114037832/video/1). The source post names the project as `syv-ai/qwen38-27b-rtx3090`; that GitHub repository now redirects to [syv-ai/HyperQwen](https://github.com/syv-ai/HyperQwen).

The posts describe a Qwen3.8-27B inference setup on one RTX 3090 with 24 GB VRAM. TeksEdge reports 82 tokens/s standard decoding, 114 with optimized MTP, and 138 with DFlash2 plus lookup drafting. The headline 381 tokens/s (about 382 in the source post) is reported for reproducing a roughly 25,000-token document already present in the prompt, using context lookup and 16-token verification—not for ordinary open-ended chat. The source post reports about 133 tokens/s on ordinary chat prompts and a reduction in time to first token from 22.4 seconds to 0.56 seconds for a repeated 25K-document query with prefix caching. Treat these as reported results, not independently reproduced benchmarks.

- Upstream (current repository): [syv-ai/HyperQwen](https://github.com/syv-ai/HyperQwen)
- Your individual fork: [benyamin-persia/HyperQwen](https://github.com/benyamin-persia/HyperQwen)
- The post's demo: [TeksEdge on X](https://x.com/TeksEdge/status/2090595990114037832/video/1)

This is a separate project and hardware setup from the earlier [TensorFold and DFlash2 post](../qwen38-tensorfold-dflash2/README.md), which concerned an M5 Pro Mac mini. Compare benchmark prompts, output overlap, quantization, concurrency, software versions, and timing methodology before treating the token rates as comparable.
