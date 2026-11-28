# llm.asm — Qwen Inference and a Bare-Metal AI OS in x86-64 Assembly

Shared by [Taqi Molavi](https://x.com/taqimolavi/status/2126408383066509502). The post links the developer's profile, [alesha-pro on GitHub](https://github.com/alesha-pro), rather than a repository URL. The matching project in that profile is [alesha-pro/llm.asm](https://github.com/alesha-pro/llm.asm), an assembly-only LLM project that runs Qwen3-0.6B, including in a small bare-metal OS.

## Upstream and your fork

| Upstream | Your individual fork | Status |
|---|---|---|
| [alesha-pro/llm.asm](https://github.com/alesha-pro/llm.asm) | [benyamin-persia/llm.asm](https://github.com/benyamin-persia/llm.asm) | Newly forked individually; GitHub parent verified as `alesha-pro/llm.asm` |

The upstream repository reports an MIT license. Its creator describes the implementation as pure x86-64 NASM, with no C/C++, Rust, libc, or runtime dependencies for its main projects. The repository includes four projects: Linux Qwen inference, a bootable bare-metal Qwen OS, a Mini-GPT trainer, and a separate Ring -1 kernel-surgeon/hypervisor project.

## What the post says, and what the repository reports

The post highlights the bare-metal Qwen3-0.6B OS: roughly 24 KB, a reported boot time around 95 ms, and 118 tokens/second at eight cores on an AMD EPYC system. It also says the project is up to 54% faster than `llama.cpp`.

The upstream README's current benchmark table reports 118.08 tokens/second for the bare-metal OS at eight threads. For comparison, it reports 80.79 tokens/second for `llama.cpp` at eight threads on its AMD EPYC 7642 setup, or +46.2% for that row. Its claimed maximum improvement across the listed CPU thread counts is +35.6% (four threads); the table's reported improvements do not substantiate the post's “up to 54%” figure as currently documented. These are upstream-reported benchmarks, not independently reproduced here; machine, model, build flags, and measurement methodology matter.

The repo also contains a separately benchmarked Linux inference engine, Mini-GPT training code, and a security-sensitive bare-metal hypervisor component. Review each subproject and its requirements before building or running it; the “zero dependencies” description does not mean the project needs no assembler, linker, model weights, suitable CPU instructions, or setup. The bare-metal OS and hypervisor should be tested only in an isolated VM or hardware you control.

## Links

- Original post: [Taqi Molavi on X](https://x.com/taqimolavi/status/2126408383066509502)
- Creator profile: [alesha-pro on GitHub](https://github.com/alesha-pro)
- Upstream project: [alesha-pro/llm.asm](https://github.com/alesha-pro/llm.asm)
- Your fork: [benyamin-persia/llm.asm](https://github.com/benyamin-persia/llm.asm)
- [Qwen3-0.6B upstream model](https://huggingface.co/Qwen/Qwen3-0.6B)
