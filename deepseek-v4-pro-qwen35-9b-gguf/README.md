# DeepSeek V4 Pro / Qwen3.5 9B Heretic GGUF

Shared in [Anya's X post](https://x.com/anya_yfa7/status/2123145473846591497): [mradermacher/DeepSeek-V4-Pro-Qwen3.5-9B-UNCENSORED-heretic-GGUF](https://huggingface.co/mradermacher/DeepSeek-V4-Pro-Qwen3.5-9B-UNCENSORED-heretic-GGUF).

This is a Hugging Face model repository, not a GitHub repository, so there is no GitHub fork to create for the checkpoint. The model card identifies it as a 9B-parameter GGUF based on Qwen3.5, with a DeepSeek V4 Pro fine-tune in its model lineage. The page labels the license Apache-2.0.

## Quantizations and local use

The model card lists Q4_K_M at 5.78 GB (rounded to 5.9 GB in its quant table), close to the post's approximate 5.7 GB claim. It also provides smaller/larger quants. File size is not total runtime memory; context and inference overhead need additional RAM/VRAM.

The Hugging Face card provides this Ollama command:

```sh
ollama run hf.co/mradermacher/DeepSeek-V4-Pro-Qwen3.5-9B-UNCENSORED-heretic-GGUF:Q4_K_M
```

It also provides instructions for llama.cpp, LM Studio, and other local runtimes. Check the model card for current quant files and compatible runtime versions before downloading.

## Claims and responsible use

The post describes the model as having strong reasoning and minimal refusals. Those are the poster's claims, not independent evaluations in this collection. The model card tags it as uncensored/abliterated; do not infer accuracy or safety from those labels. Review outputs, use suitable safeguards, and follow the model license and applicable law.
