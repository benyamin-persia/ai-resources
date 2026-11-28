# LLM.OS — Local Qwen Inference in a Browser

Shared by [Konark Modi](https://x.com/konarkmodi/status/2126462416426815848). The post links the [LLM.OS experiment](https://tesseracted.com/experiments-llm-os): a browser terminal that runs quantized Qwen models locally through WebAssembly, without an inference server or API key. The author describes the demo as experimental and says it may fail.

## What the post links and mentions

1. **LLM.OS browser demo:** [tesseracted.com/experiments-llm-os](https://tesseracted.com/experiments-llm-os) — runnable website from Tesseracted Labs; no public GitHub source repository for this demo is linked on the page.
2. **llm.asm:** [alesha-pro/llm.asm](https://github.com/alesha-pro/llm.asm) — the assembly inference project that inspired the WebAssembly engine. Your individual fork already exists at [benyamin-persia/llm.asm](https://github.com/benyamin-persia/llm.asm), and was previously parent-verified. See the [llm.asm catalog entry](../llm-asm/README.md).
3. **unkernel:** [unkernel.dev](https://unkernel.dev) — a separate real Linux kernel running in WebAssembly, cited as inspiration. Its site links the source repository [pithings/unkernel](https://github.com/pithings/unkernel), which has now been forked individually to [benyamin-persia/unkernel](https://github.com/benyamin-persia/unkernel). GitHub confirms the personal fork's parent is `pithings/unkernel`. GitHub reports the repository's license as GPL-2.0, while the website HTML includes an MIT SPDX comment; check the actual license files and scope before reuse rather than assuming the site and repository share one license.
4. **Model/weight attribution:** the post mentions Qwen and Unsloth-quantized weights. The demo currently lists Qwen3 and Qwen3.5 model variants and says it uses Unsloth Q4_K_M GGUF weights converted for its engine. These are model/weight resources rather than GitHub repositories to fork. The page credits [Pyodide](https://pyodide.org) for its optional in-browser Python sandbox.

## What the demo page reports

The post describes a roughly 40 KB WebAssembly engine and about 50 tokens/second. The live experiment page now describes its engine as approximately 52–55 KB, and its current benchmark table reports results on an Apple M3 Max: about 52 tokens/second for Qwen3-1.7B and about 124 tokens/second for Qwen3-0.6B, both using eight threads. It compares those results with native `llama.cpp` CPU and GPU numbers. Treat all speed and correctness figures as the author's measurements; they vary by browser, device, model, build, and settings. The page says its faster quantized path can differ from the exact path and can sometimes select different tokens.

The demo downloads model weights into the browser and computes tokens locally; the weights are much larger than the engine itself. The page reports memory use from roughly 0.6 GB for the smaller models to around 1.4 GB for Qwen3.5-2B, so “40 KB” or “52 KB” refers to the engine binary, not the entire model. The page says prompts and replies stay in the tab and are not sent to an inference server, while Cloudflare page analytics still receives page/browser metadata. Its own caveats: small models can confidently produce incorrect answers, browser background throttling can slow generation, and the optional Python sandbox has a 15-second limit and no network access.

## Individual GitHub fork results

| Upstream repository | Your fork | Result |
|---|---|---|
| [alesha-pro/llm.asm](https://github.com/alesha-pro/llm.asm) | [benyamin-persia/llm.asm](https://github.com/benyamin-persia/llm.asm) | Existing fork; parent verified |
| [pithings/unkernel](https://github.com/pithings/unkernel) | [benyamin-persia/unkernel](https://github.com/benyamin-persia/unkernel) | Newly forked individually; parent verified; GitHub reports GPL-2.0 |

No duplicate fork was made for `llm.asm`. No fork was made for the LLM.OS website, Pyodide, or model weights because the source provides no GitHub repository for the LLM.OS demo and those other links are not GitHub repositories.

## Links

- [Original X post](https://x.com/konarkmodi/status/2126462416426815848)
- [LLM.OS browser experiment](https://tesseracted.com/experiments-llm-os)
- [Tesseracted Labs](https://tesseracted.com/)
- [llm.asm upstream](https://github.com/alesha-pro/llm.asm) · [your fork](https://github.com/benyamin-persia/llm.asm)
- [unkernel website](https://unkernel.dev) · [upstream source](https://github.com/pithings/unkernel) · [your fork](https://github.com/benyamin-persia/unkernel)
- [Pyodide](https://pyodide.org)
