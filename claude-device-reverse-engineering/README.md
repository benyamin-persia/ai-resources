# Reverse-Engineering Devices with Claude Code

Collected from [Cabbitar's X post](https://x.com/cabbitar/status/2119392619327590507) and its linked article, [How To Reverse Engineer Any Device With Claude Code](https://x.com/i/article/2119163597905682433). The article presents REA as the agent hub, with specialist tools for firmware, apps, binaries, and network traffic, plus prompts and workspace guardrails. It says to examine only devices and software you own or are authorized to inspect; network captures can contain sensitive data.

## All 18 GitHub projects

### Agent hub and clean-room workflow

- [REA](https://github.com/morluto/rea) → [your fork](https://github.com/benyamin-persia/rea) — MCP-based app and binary analysis; already forked.
- [Ghidra](https://github.com/NationalSecurityAgency/ghidra) → [your fork](https://github.com/benyamin-persia/ghidra) — software reverse-engineering framework; already forked.
- [GhidraMCP](https://github.com/LaurieWired/GhidraMCP) → [your fork](https://github.com/benyamin-persia/GhidraMCP) — MCP bridge for driving Ghidra.
- [Craft Anything](https://github.com/storytold/craft-anything) → [your fork](https://github.com/benyamin-persia/craft-anything) — agent workflow for studying behavior, making an independent implementation, and verifying it; already forked.

### Binary analysis and debugging

- [radare2](https://github.com/radareorg/radare2) → [your fork](https://github.com/benyamin-persia/radare2) — command-line reverse-engineering framework.
- [rizin](https://github.com/rizinorg/rizin) → [your fork](https://github.com/benyamin-persia/rizin) — reverse-engineering framework and radare2 fork.
- [x64dbg](https://github.com/x64dbg/x64dbg) → [your fork](https://github.com/benyamin-persia/x64dbg) — Windows debugger.
- [RAD Debugger](https://github.com/EpicGames/raddebugger) → [your fork](https://github.com/benyamin-persia/raddebugger) — debugger for native applications.
- [ImHex](https://github.com/WerWolv/ImHex) → [your fork](https://github.com/benyamin-persia/ImHex) — hex editor with pattern-language support.
- [angr](https://github.com/angr/angr) → [your fork](https://github.com/benyamin-persia/angr) — binary analysis and symbolic-execution framework.

### Mobile and managed applications

- [jadx](https://github.com/skylot/jadx) → [your fork](https://github.com/benyamin-persia/jadx) — Android DEX decompiler; already forked.
- [Apktool](https://github.com/iBotPeaches/Apktool) → [your fork](https://github.com/benyamin-persia/Apktool) — Android APK resource decoder and builder.
- [Frida](https://github.com/frida/frida) → [your fork](https://github.com/benyamin-persia/frida) — dynamic instrumentation toolkit.
- [ILSpy](https://github.com/icsharpcode/ILSpy) → [your fork](https://github.com/benyamin-persia/ILSpy) — .NET assembly browser and decompiler; already forked.
- [dnSpy](https://github.com/dnSpyEx/dnSpy) → [your fork](https://github.com/benyamin-persia/dnSpy) — .NET debugger and assembly editor.

### Network inspection and resource indexes

- [mitmproxy](https://github.com/mitmproxy/mitmproxy) → [your fork](https://github.com/benyamin-persia/mitmproxy) — interactive HTTPS proxy for inspecting traffic.
- [awesome-reverse-engineering](https://github.com/morluto/awesome-reverse-engineering) → [your fork](https://github.com/benyamin-persia/awesome-reverse-engineering) — curated reverse-engineering resources; already forked.
- [awesome-ai-reverse-engineering](https://github.com/zhuyansen/awesome-ai-reverse-engineering) → [your fork](https://github.com/benyamin-persia/awesome-ai-reverse-engineering) — index of AI-assisted reverse-engineering projects.

I checked all 18 upstreams against your account: 12 missing repositories were forked individually and verified; the other 6 were already forks. The article's install commands and compatibility notes are its own guidance—check each upstream's current documentation, platform support, and license before use.
