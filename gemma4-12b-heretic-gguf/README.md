# Gemma 4 12B Heretic Abliterated GGUF

From [Mingzi206's X post](https://x.com/mingzi206/status/2123081535914213723), which recommends this Hugging Face checkpoint for local inference, including on consumer GPUs. The post links to a model page, not a GitHub repository.

- Model: [culturerevolt/gemma-4-12b-heretic-abliterated-GGUF](https://huggingface.co/culturerevolt/gemma-4-12b-heretic-abliterated-GGUF)
- Model family: Gemma 4 12B Heretic, distributed in GGUF quantizations.
- Your existing runtime fork: [benyamin-persia/ollama](https://github.com/benyamin-persia/ollama) → upstream [ollama/ollama](https://github.com/ollama/ollama). No new GitHub fork is needed for this post; the model checkpoint itself is hosted on Hugging Face.

The Hugging Face page currently shows 105,435 downloads over the last month and lists the model as Apache-2.0 licensed. Download counts change over time. The post's assertions about refusal behavior, preserved reasoning/multimodal capability, and popularity are promotional claims, not independently evaluated here.

## Quantization and hardware

The model card's current file-size table lists IQ3_XS at 5.27 GB, IQ4_XS at 6.64 GB, Q4_K_M at 7.38 GB, Q5_K_M at 8.55 GB, Q6_K at 9.79 GB, and Q8_0 at 12.7 GB. Its own hardware guidance places IQ3_XS at 8–12 GB VRAM, IQ4_XS at 12–16 GB, and Q4_K_M at 16 GB. Weight-file size is not the same as total runtime VRAM: context/KV cache and runtime overhead also use memory. Check the model card and test the quant that fits your machine rather than assuming every 7–8 GB file will fit in 12 GB VRAM.

The card gives this Ollama example for Q4_K_M:

```sh
ollama run hf.co/culturerevolt/gemma-4-12b-heretic-abliterated-GGUF:Q4_K_M
```

The X post also mentions LM Studio; consult its current model import and hardware documentation for that runtime.

## Use and safety notes

The card describes this as an abliterated/uncensored model and warns that it may generate unfiltered output; it recommends responsible use in local sandbox development setups. Do not treat an “uncensored” label as evidence of accuracy, capability, or safety. Keep human review and appropriate safeguards around applications that expose model output to other people, and follow applicable laws and the model's license.
