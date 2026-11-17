# 11 Repositories for Research-to-Voice Production

The 11 GitHub repositories from [Roundtable Space's X post](https://x.com/RoundtableSpace/status/2122581753449845217), organized in the workflow order research → writing → slides → video → voice. Each upstream is paired with your individual fork. The first repository, `last30days-skill`, was also featured in a later [HazratCrypto post](https://x.com/HazratCrypto/status/2122690532740661724), which describes searching Reddit, X, YouTube, Hacker News, and Polymarket for the past 30 days and returning a sourced summary. The post's star count and tool compatibility claims are not independently verified here.

| # | Stage | Repository | Purpose from the post | License as stated in post | Upstream | Your fork |
|---:|---|---|---|---|---|---|
| 1 | Research | last30days-skill | Research a topic across Reddit, YouTube, Hacker News, and the web. | MIT | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | [last30days-skill](https://github.com/benyamin-persia/last30days-skill) |
| 2 | Video understanding | claude-video | Ask questions about a video Claude has watched. | MIT | [bradautomates/claude-video](https://github.com/bradautomates/claude-video) | [claude-video](https://github.com/benyamin-persia/claude-video) |
| 3 | Writing | humanizer | Revise drafts to reduce signs of AI-generated prose. | MIT | [blader/humanizer](https://github.com/blader/humanizer) | [humanizer](https://github.com/benyamin-persia/humanizer) |
| 4 | Slides | frontend-slides | Create animated HTML slides from a prompt or PowerPoint. | MIT | [zarazhangrui/frontend-slides](https://github.com/zarazhangrui/frontend-slides) | [frontend-slides](https://github.com/benyamin-persia/frontend-slides) |
| 5 | Slides & narration | ppt-master | Turn documents into editable PowerPoint decks with speaker-note narration. | MIT | [hugohe3/ppt-master](https://github.com/hugohe3/ppt-master) | [ppt-master](https://github.com/benyamin-persia/ppt-master) |
| 6 | Video rendering | HyperFrames | Write HTML scenes and render them as video. | Apache-2.0 | [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) | [hyperframes](https://github.com/benyamin-persia/hyperframes) |
| 7 | Video editing | video-use | Edit raw footage conversationally; the post says it requires an ElevenLabs key. | MIT | [browser-use/video-use](https://github.com/browser-use/video-use) | [video-use](https://github.com/benyamin-persia/video-use) |
| 8 | Video production | OpenMontage | Let a coding agent run a video-production workflow. | AGPL-3.0 | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | [OpenMontage](https://github.com/benyamin-persia/OpenMontage) |
| 9 | Text to speech | Pocket TTS | Generate speech on a CPU. | MIT code | [kyutai-labs/pocket-tts](https://github.com/kyutai-labs/pocket-tts) | [pocket-tts](https://github.com/benyamin-persia/pocket-tts) |
| 10 | Text to speech | Phonon / xn-ptts | On-device text-to-speech; the post notes multilingual weights are non-commercial. | Apache-2.0 code; non-commercial weights | [gradium-ai/xn-ptts](https://github.com/gradium-ai/xn-ptts) | [xn-ptts](https://github.com/benyamin-persia/xn-ptts) |
| 11 | Voice cloning | ZONOS3-Mini | Text-to-speech with voice cloning in multiple languages. | Apache-2.0 weights, per post | [Zyphra/ZONOS3-Mini](https://github.com/Zyphra/ZONOS3-Mini) | [ZONOS3-Mini](https://github.com/benyamin-persia/ZONOS3-Mini) |

Seven forks were created for this post; last30days-skill, humanizer, HyperFrames, and video-use were already forked in your account. The post advises checking each project's actual license and cloning a voice only with the speaker's consent. License labels above are transcribed from the post; verify current code, model-weight, and asset licenses at each upstream before use.

Machine-readable list: [`repositories.json`](repositories.json) · [Upstream URLs](upstreams.txt) · [Fork URLs](forks.txt)
