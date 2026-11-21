# Strata — Run Qwen3.8-Flash-Next Locally

Shared by [HazratCrypto on X](https://x.com/HazratCrypto/status/2123990382123848073). [Strata](https://github.com/Niko1221/Strata) is an open-source inference engine and desktop/terminal app for running Qwen3.8-Flash-Next and other supported models locally. The upstream README describes local OpenAI- and Anthropic-compatible APIs for coding tools including Codex and Claude Code; its current model list also includes Cursor-compatible usage through its API endpoint.

Your individual fork: [benyamin-persia/Strata](https://github.com/benyamin-persia/Strata), forked from [Niko1221/Strata](https://github.com/Niko1221/Strata). The upstream currently reports the 0.2.17 release.

## Hardware caveat

The post highlights running the 125B model with a 12 GB GPU, but GPU memory is not the whole requirement. Strata's [model sizing guide](https://github.com/Niko1221/Strata/blob/main/docs/MODELS.md) gives combined system-RAM-plus-VRAM estimates of roughly 37.6–54.8 GB for its listed Qwen3.8-Flash-Next sizes; smaller-memory configurations can read more experts from disk and run much slower. The smaller model packs themselves require roughly 66–76 GB of downloads, with an additional MTP draft layer on first launch. Check the current sizing guide and the launch plan for your specific machine before downloading.

The upstream [safety and privacy notes](https://github.com/Niko1221/Strata/blob/main/docs/SAFETY.md) say Strata has no telemetry and that local chats stay on-device; they also explain that external model services, web tools, and connected coding agents can send data to their own services. Review those boundaries, plus the selected model's license and data terms.
