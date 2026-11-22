# Cutaway — Image-to-3D Exploded Films

[Cutaway](https://github.com/Nyxera0x/cutaway) is a Claude Code skill that uses a reference image to build a stylized, code-generated three.js object, then create an exploded-view animation/film. Its docs describe a review loop and include three sample builds. This is an interpretation of an image, not an exact engineering reconstruction.

- Source post: [HazratCrypto on X](https://x.com/HazratCrypto/status/2124231300181553654)
- Upstream: [Nyxera0x/cutaway](https://github.com/Nyxera0x/cutaway)
- Your individual fork: [benyamin-persia/cutaway](https://github.com/benyamin-persia/cutaway)
- License: MIT, per the upstream README

Install for Claude Code:

```sh
npx skills add Nyxera0x/cutaway -g -a claude-code
```

Then, once in the installed folder:

```sh
npm install && npx playwright install chromium
```

Requirements noted upstream: Node.js 20+, FFmpeg for video, and Python 3 for sound. A sample can be built without an agent with `node sims/build.mjs tarantula-film`. Review the upstream docs for the full workflow and current requirements.
