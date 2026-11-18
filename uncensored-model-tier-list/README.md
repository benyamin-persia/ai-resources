# Uncensored Model Tier List

The 20 use-case picks from [Av1dlive's X post](https://x.com/Av1dlive/status/2122755432599142890), preserved as the poster's recommendations—not independent evaluations or verified benchmark rankings.

Structured list: [models.json](models.json)

| Use case | Model named in the post |
|---|---|
| Best overall | Qwen3.8 27B Abliterated |
| Hosted | DeepSeek V4.1 Flash Uncensored (Venice) |
| Small GPU | Gemma 4 12B Uncensored |
| Fast | Qwen3.6 35B-A3B Heretic |
| Agents | Qwen3.8 27B Abliterated |
| Writing | Gemma 4 26B-A4B Ultra Heretic |
| Roleplay | Cydonia 24B v4.3 |
| Natural (no surgery) | Hermes 4.3 36B |
| Reasoning | Gemma 4 31B Heretic |
| Vision | Gemma 4 Heretic (size/checkpoint not specified) |
| Coding | Qwen3-Coder 30B-A3B Abliterated |
| Laptop | Gemma 4 E2B Heretic |
| Biggest | GLM 4.6 Derestricted v3 |
| Image generation | Qwen-Image 2.1 |
| Image editing | Qwen-Image-Edit 2511 |
| Video | Wan 2.2 |
| Long context | GLM 5.3 Flash Uncensored (Venice) |
| Research | DeepSeek V4.1 Flash Uncensored (Venice) |
| Security | GLM-5.3 Flash Cybersecurity |
| Phone | PocketPal AI + Gemma 4 E2B Heretic |

The post points to the Hugging Face publisher accounts [huihui-ai](https://huggingface.co/huihui-ai), [llmfan46](https://huggingface.co/llmfan46), [TheDrummer](https://huggingface.co/TheDrummer), and [NousResearch](https://huggingface.co/NousResearch), or [Venice](https://venice.ai/) for hosted access. It does not provide exact model-card URLs, quantizations, or consistent checkpoint IDs, so this list cannot identify every recommended download unambiguously. The same Qwen model is listed for overall and agent use; the same DeepSeek model appears for hosted and research use.

## Setup mentioned in the post

The post gives generic Ollama/Hugging Face commands with placeholders:

```text
ollama pull hf.co/<user>/<repo>:<quant>
ollama run hf.co/<user>/<repo>:<quant>
/set nothink
```

These are recorded as the post's instructions, not validated against each model or the current Ollama CLI. Confirm the exact model ID, quantization, license, hardware needs, and current command syntax before downloading. Models can produce incorrect or unsafe output; do not treat an uncensored label or this tier list as a reliability or security rating.

PocketPal AI is the phone app named by the post: [upstream](https://github.com/a-ghorbani/pocketpal-ai) · [your individual fork](https://github.com/benyamin-persia/pocketpal-ai). The post does not link GitHub repositories for the model checkpoints. Ollama is used in its setup, and your existing [Ollama fork](https://github.com/benyamin-persia/ollama) is already in the collection.

For another broad model directory from your saved posts, see [Every Free Uncensored AI Model](../uncensored-ai-free/README.md).
