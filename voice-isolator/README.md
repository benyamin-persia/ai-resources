# Inworld Voice Isolator

Shared in [The_MissAI's X post](https://x.com/The_MissAI/status/2125448358743388660). Inworld's open-source, Apache-2.0 project separates speech from background noise in recorded audio and live streams. The upstream provides offline and low-latency streaming models, a Python package, CLI, and interactive demo; it produces 48 kHz audio.

- Upstream: [inworld-ai/voice-isolator](https://github.com/inworld-ai/voice-isolator)
- Your individual fork: [benyamin-persia/voice-isolator](https://github.com/benyamin-persia/voice-isolator)
- Model weights: [inworld/voice-isolator on Hugging Face](https://huggingface.co/inworld/voice-isolator)
- Install: `pip install inworld-voice-isolation`
- Requirements: Python 3.10+ and PyTorch 2.1+; upstream says it runs on CPU, CUDA GPUs, and Apple Silicon's MPS backend.

Scope note: this is voice isolation, not speaker selection or audio restoration. The live demo streams microphone input, but the project is a developer-oriented package/demo rather than a one-click desktop app. Upstream says hardware coverage for smaller GPUs is not yet tested; check its current hardware notes before relying on performance.
