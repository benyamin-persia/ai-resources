# Qwen3.8-35B-A3B on an RTX 3060: Local Inference Notes

Shared in [Oluwaphilemon1's X post](https://x.com/Oluwaphilemon1/status/2122470941842166127), which links to a [demonstration video](https://x.com/DogukanUrker/status/2100346050473074805/video/1).

The post describes a reported local setup using Qwen3.8-35B-A3B, `llama.cpp`, a 12 GB RTX 3060, and 16 GB system RAM. It attributes the setup to Q4_K_M quantization, CPU offload for 26 MoE layers, Flash Attention, and an 8-bit KV cache, and reports roughly 50 tokens/s generation and 550 tokens/s prompt processing. These are claims from the post, not independently verified benchmarks or hardware guarantees. Prefill and decode are different measurements; the higher prefill figure is not the response-generation rate.

The article explains the approach as a combination of sparse Mixture-of-Experts compute, quantization, CPU/GPU memory sharing, and inference optimizations. It does not link the model checkpoint. It mentions `llama.cpp` but does not link its repository; the official [ggml-org/llama.cpp](https://github.com/ggml-org/llama.cpp) upstream is included here for reference, and your existing fork is [benyamin-persia/llama.cpp](https://github.com/benyamin-persia/llama.cpp).

Check the linked post/video, model card, and current llama.cpp documentation for the exact model, build flags, memory use, compatibility, and benchmark method before attempting to reproduce the reported results.
