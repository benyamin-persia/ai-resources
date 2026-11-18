# Gemma 4 E4B Heretic GGUF on Ollama

From [DeRonin_'s X walkthrough](https://x.com/DeRonin_/status/2122674029932753076), which describes running an abliterated Gemma GGUF on CPU or older GPUs using Ollama. The post links to the [Ollama installer](https://ollama.com/) and this [Hugging Face model](https://huggingface.co/igorls/gemma-4-E4B-it-qat-q4_0-unquantized-heretic-GGUF); it does not directly link a GitHub repository. Your [Ollama fork](https://github.com/benyamin-persia/ollama) already exists and points to [ollama/ollama](https://github.com/ollama/ollama).

## Post's workflow

The post's seven-step outline is:

1. Install Ollama.
2. Choose a model size that fits available RAM/VRAM.
3. Pull the linked Gemma 4 E4B Heretic GGUF.
4. Disable thinking (the post suggests `/set nothink`).
5. Keep the context window small (it suggests 8,192 tokens).
6. Optionally enable flash attention and quantized KV cache.
7. Check CPU/GPU allocation and token speed with `ollama ps` and verbose output.

The post's advertised hardware fit, speeds, benchmark/refusal numbers, and “$0” claim are the author's claims, not measurements verified here. Actual speed and memory use depend on model/runtime versions, hardware, drivers, context length, and other settings.

## Check the model card before using the post's command

The current [Hugging Face model card](https://huggingface.co/igorls/gemma-4-E4B-it-qat-q4_0-unquantized-heretic-GGUF) documents `Q4_0` (about 4.8 GB in its quant table) and `Q8_0` (about 7.4 GB), and provides this Ollama command:

```sh
ollama run hf.co/igorls/gemma-4-E4B-it-qat-q4_0-unquantized-heretic-GGUF:Q4_0
```

The X post instead appends `:Q4_K_M`; that tag is not documented on the card. The card also says the build was abliterated/evaluated with thinking enabled, so the post's `/set nothink` advice is not confirmed by the linked model documentation. Check the model card and your installed Ollama version before relying on those exact commands. The card labels this checkpoint as 7B parameters; its tags/name say E4B, so avoid treating the post's memory estimates as guaranteed.

## Safety and licensing

The model card labels the license Apache 2.0 and explicitly warns that this is an abliterated model with deliberately removed refusal behavior. It may produce offensive, inaccurate, explicit, or harmful output; the card advises applying your own safeguards and human review before production or user-facing use. Use it lawfully and responsibly, and do not assume local inference makes every surrounding tool or integration private.

No new GitHub fork was needed for this post: its model checkpoint is hosted on Hugging Face, and the related Ollama GitHub project was already forked individually.
