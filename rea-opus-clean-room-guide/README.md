# REA, Oracles & Clean-Room Reverse-Engineering Guide

Collected from [N01ennn's X post](https://x.com/N01ennn/status/2110319993128706208) and its linked [article](https://x.com/i/article/2109686434210693120), “How to Turn Opus 5.5 Into a Reverse Engineer: The Full Guide to REA, Oracles and Clean-Room Loops.” The article describes using REA to inspect software behavior, record evidence-backed specifications, implement independently, and test against carefully designed behavioral oracles. Its examples include Windows Calculator percentage behavior and an open-source Touhou 8 reconstruction. Model capability/version claims are the article's, not independently validated here.

## Linked GitHub projects — individually forked

- [REA](https://github.com/morluto/rea) → [your fork](https://github.com/benyamin-persia/rea) — agent tooling for observing application behavior and tracing actions to code; this individual fork already existed.
- [FilmCraft](https://github.com/storytold/filmcraft) → [your fork](https://github.com/benyamin-persia/filmcraft) — open-source nonlinear video editor written in Rust.
- [LightCraft](https://github.com/storytold/lightcraft) → [your fork](https://github.com/benyamin-persia/lightcraft) — non-destructive photo editor written in Rust.
- [PhotoCraft](https://github.com/storytold/photocraft) → [your fork](https://github.com/benyamin-persia/photocraft) — open-source photo editor written in Rust.
- [Ghidra](https://github.com/NationalSecurityAgency/ghidra) → [your fork](https://github.com/benyamin-persia/ghidra) — software reverse-engineering framework, referenced in the article's native-binary workflow.
- [Touhou 8 source reconstruction](https://github.com/N0zoM1z0/th08) → [your fork](https://github.com/benyamin-persia/th08) — repository linked by an example pull request in the article.

The article advocates separating observed behavior from inference and unknowns, writing a behavior-only specification before implementation, and checking edge cases with oracles. It explicitly recommends not copying original code, addresses, names, or assets. Use these methods only with software you are authorized to inspect; respect applicable law, licenses, terms, access controls, and privacy.
