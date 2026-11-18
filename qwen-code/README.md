# Qwen Code

Collected from [HazratCrypto's X post](https://x.com/HazratCrypto/status/2122839916363096078).

- Upstream: [QwenLM/qwen-code](https://github.com/QwenLM/qwen-code)
- Your individual fork: [benyamin-persia/qwen-code](https://github.com/benyamin-persia/qwen-code)
- Install method shown in the post: `npm install -g @qwen-code/qwen-code@latest`; then run `qwen` inside a project.

The upstream README currently labels version 1.0 as a preview, lists Node.js 22+ for the npm installation, and says Qwen Code can use Qwen, OpenAI, Anthropic, Gemini, third-party APIs, or local models through Ollama/vLLM. The chosen provider determines whether usage requires a subscription/API key or can run locally; selecting Qwen Code alone does not make a cloud provider free or local.

The post's SWE-bench claim is close to the current upstream evaluation summary: the README reports 76.40%–77.80% averages across seven Qwen Code versions using Qwen 3.7 Max, 500 tasks, and three trials per version. Treat this as the project's reported evaluation, not an independent benchmark.

The post also says free Qwen-account access was discontinued and Plus/Pro or a personal API key is needed. The upstream quick start currently lists a Qwen subscription or configuring a provider API key for hosted authentication; check the current docs and provider terms before relying on pricing or access claims.

Security note: the upstream README says its experimental daemon binds to loopback without bearer authentication by default, and local processes that can reach it can use its API, including code execution. On shared or untrusted machines, review the upstream security instructions and configure authentication before exposing it.
