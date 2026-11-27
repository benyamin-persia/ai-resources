# AI Resources: What This Project Is, What We Do, and How to Continue

This document is the handoff for the ongoing resource-curation workflow. It explains the purpose of this repository, the exact meaning of “fork them all one by one,” what has been done, where the source and project links live, and a reusable prompt for continuing the same work when new links arrive.

## The project in one sentence

We are building [benyamin-persia/ai-resources](https://github.com/benyamin-persia/ai-resources), a categorized, source-attributed library of AI, agent, design, video, developer, and learning resources shared by the user, while individually forking every relevant GitHub repository linked by those sources that is not already forked in the user's account.

This is both a catalog and a set of personal GitHub forks. A link sent to the assistant is an instruction to investigate and process it, not merely to save its URL.

## What the repeated workflow does

For each source URL the user sends:

1. **Identify the actual source and its contents.** Open the X post, article, website, GitHub repository, or other supplied page. Extract the resources it actually links to. Do not guess at missing links or silently substitute a different project. If X is unavailable, use reliable accessible copies or linked material where possible and clearly note the limitation.
2. **Process the resources individually and in source order.** For a post that lists repositories, inspect each repository one by one. Preserve source ordering and the source's categories where that helps reproduce a tutorial or list faithfully. Do not collapse multiple repositories into a generic “collection” entry.
3. **Classify each item.** Distinguish GitHub repositories from websites, hosted services, papers, Hugging Face models, videos, prompts, and skills/catalog entries. Only actual GitHub repositories can be forked. Non-GitHub resources are recorded with their canonical links and useful context, never represented as forks.
4. **Check each GitHub fork relationship.** Look for the user's repository at `https://github.com/benyamin-persia/<repo>`. Verify its GitHub parent relationship (`parent.full_name`) instead of relying on a matching name. A same-named repository is not automatically a fork. If a correct fork already exists, keep it and link it. If it does not, create that one fork individually, then verify its parent. Do this for every repository in the source.
5. **Record provenance, not just a URL.** Add the original post/article, canonical upstream, the user's fork when one exists, a concise description, and important license, availability, hardware, privacy, safety, or accuracy caveats. Attribute claims to their source; do not present promotional claims as independently verified facts.
6. **Add a focused detail page and index it.** Each post or coherent resource batch normally gets a dedicated Markdown page/folder. Add that page to the appropriate category in [`README.md`](README.md), which serves as the main catalog. Related/duplicate posts should be cross-referenced rather than creating confusing duplicate project entries.
7. **Check, commit, push, and report.** Review the diff, run `git diff --check`, commit the catalog and indexing changes, push to `origin`, and verify that the push succeeded. In the handoff, state what was added, how many forks were already present versus newly created, and any unavailable or unverified items.

## What “fork them all one by one” means here

“One by one” means every distinct GitHub repository in a supplied source gets an explicit upstream → personal-fork record and an individual existence/parent check. It does **not** mean making duplicate forks when the correct fork already exists. Existing forks count as processed only after verification. New forks are created separately, one upstream at a time—not replaced with a single umbrella repository and not silently skipped because a list is long.

Keep the forks in the user's GitHub account and the catalog pages in `ai-resources` as two distinct deliverables:

- The catalog page records what the source said, the canonical upstream, and the matching personal fork.
- The actual GitHub fork is the user's separate repository derived from that upstream.
- The `ai-resources` repository is not a mirror of every project's code. It indexes those projects and links to each individual fork.

If GitHub access, rate limits, permissions, a deleted repository, or an unavailable source prevents an action, report the exact item and stop claiming it is complete. Never label an ordinary repository as a fork without confirming GitHub's parent metadata.

## Where the catalog lives

- Main index and categories: [`README.md`](README.md)
- Complete per-source detail pages: the linked Markdown pages under the folders listed below and throughout the main index.
- Remote repository: [github.com/benyamin-persia/ai-resources](https://github.com/benyamin-persia/ai-resources)
- Personal fork namespace: [github.com/benyamin-persia](https://github.com/benyamin-persia)

The main README links to the full existing catalog: agent frameworks, workflow and design repositories, video/animation stacks, model pages, skills, developer platforms, desktop tools, learning material, and website collections. The per-source pages retain the complete ordered lists, exact upstream/fork pairs, machine-readable exports where present, and the original post/article links. Start from the main README when looking for older work; do not make up a second list or re-fork its entries.

## Latest work recorded in the repository

The most recent set of commits covers the following source batches. Each source page linked here has the item-level details; the fork tables below make the one-by-one fork work explicit.

### Creative animation and production: 13 repositories

Source: [0xCarrera's X post](https://x.com/0xCarrera/status/2125950726136328524) · Catalog: [`13-animation-repositories-carrera/README.md`](13-animation-repositories-carrera/README.md) · Commit: `e2b5e1e` (`Catalog Carrera's animation repositories`).

All 13 upstreams were checked against the individual personal forks. Ten forks already existed; three were newly created individually:

| # | Upstream | Personal fork | Status in this batch |
|---:|---|---|---|
| 1 | [storytold/photocraft](https://github.com/storytold/photocraft) | [benyamin-persia/photocraft](https://github.com/benyamin-persia/photocraft) | Already existed; verified |
| 2 | [Leonxlnx/earshot](https://github.com/Leonxlnx/earshot) | [benyamin-persia/earshot](https://github.com/benyamin-persia/earshot) | Already existed; verified |
| 3 | [lemomo-ai/lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) | [benyamin-persia/lemo-opuscar](https://github.com/benyamin-persia/lemo-opuscar) | Newly forked individually |
| 4 | [feitangyuan/onetake](https://github.com/feitangyuan/onetake) | [benyamin-persia/onetake](https://github.com/benyamin-persia/onetake) | Newly forked individually |
| 5 | [wesbos/3d-model-anything](https://github.com/wesbos/3d-model-anything) | [benyamin-persia/3d-model-anything](https://github.com/benyamin-persia/3d-model-anything) | Newly forked individually |
| 6 | [Alchemist0823/three.quarks](https://github.com/Alchemist0823/three.quarks) | [benyamin-persia/three.quarks](https://github.com/benyamin-persia/three.quarks) | Already existed; verified |
| 7 | [greensock/GSAP](https://github.com/greensock/GSAP) | [benyamin-persia/GSAP](https://github.com/benyamin-persia/GSAP) | Already existed; verified |
| 8 | [mrdoob/three.js](https://github.com/mrdoob/three.js) | [benyamin-persia/three.js](https://github.com/benyamin-persia/three.js) | Already existed; verified |
| 9 | [ahujasid/mcp-for-blender](https://github.com/ahujasid/mcp-for-blender) | [benyamin-persia/mcp-for-blender](https://github.com/benyamin-persia/mcp-for-blender) | Already existed; verified |
| 10 | [Comfy-Org/ComfyUI](https://github.com/Comfy-Org/ComfyUI) | [benyamin-persia/ComfyUI](https://github.com/benyamin-persia/ComfyUI) | Already existed; verified |
| 11 | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | [benyamin-persia/taste-skill](https://github.com/benyamin-persia/taste-skill) | Already existed; verified |
| 12 | [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) | [benyamin-persia/hyperframes](https://github.com/benyamin-persia/hyperframes) | Already existed; verified |
| 13 | [remotion-dev/remotion](https://github.com/remotion-dev/remotion) | [benyamin-persia/remotion](https://github.com/benyamin-persia/remotion) | Already existed; verified |

### Web data and research: 9 repositories

Source: [smratitiwa86867's X post](https://x.com/smratitiwa86867/status/2126017593874194916) · Catalog: [`9-web-data-tools-smrati/README.md`](9-web-data-tools-smrati/README.md) · Commit: `0605dde` (`Catalog nine web data extraction repositories`).

All nine upstreams were paired with the verified personal forks. Firecrawl and Oxylabs Web API MCP already existed; the other seven were individually forked for this collection.

| # | Upstream | Personal fork | Status in this batch |
|---:|---|---|---|
| 1 | [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | [benyamin-persia/firecrawl](https://github.com/benyamin-persia/firecrawl) | Already existed; verified |
| 2 | [unclecode/crawl4ai](https://github.com/unclecode/crawl4ai) | [benyamin-persia/crawl4ai](https://github.com/benyamin-persia/crawl4ai) | Newly forked individually |
| 3 | [scrapy/scrapy](https://github.com/scrapy/scrapy) | [benyamin-persia/scrapy](https://github.com/benyamin-persia/scrapy) | Newly forked individually |
| 4 | [microsoft/playwright](https://github.com/microsoft/playwright) | [benyamin-persia/playwright](https://github.com/benyamin-persia/playwright) | Newly forked individually |
| 5 | [browserless/browserless](https://github.com/browserless/browserless) | [benyamin-persia/browserless](https://github.com/benyamin-persia/browserless) | Newly forked individually |
| 6 | [AndyTheFactory/newspaper4k](https://github.com/AndyTheFactory/newspaper4k) | [benyamin-persia/newspaper4k](https://github.com/benyamin-persia/newspaper4k) | Newly forked individually |
| 7 | [adbar/trafilatura](https://github.com/adbar/trafilatura) | [benyamin-persia/trafilatura](https://github.com/benyamin-persia/trafilatura) | Newly forked individually |
| 8 | [oxylabs/web-api-mcp](https://github.com/oxylabs/web-api-mcp) | [benyamin-persia/web-api-mcp](https://github.com/benyamin-persia/web-api-mcp) | Already existed; verified |
| 9 | [gocolly/colly](https://github.com/gocolly/colly) | [benyamin-persia/colly](https://github.com/benyamin-persia/colly) | Newly forked individually |

### Five AI repositories

Source: [Shoumya23's X post](https://x.com/Shoumya23/status/2126010943226483184) · Catalog: [`5-ai-repositories-shoumya/README.md`](5-ai-repositories-shoumya/README.md) · Commit: `7ae4c94` (`Catalog Shoumya's five AI repositories`).

All five relationships were verified. MiniMind, Univer, and Claude-BugHunter were newly forked; Last30Days Skill and FFmpeg Skill already had personal forks.

| # | Upstream | Personal fork | Status in this batch |
|---:|---|---|---|
| 1 | [jingyaogong/minimind](https://github.com/jingyaogong/minimind) | [benyamin-persia/minimind](https://github.com/benyamin-persia/minimind) | Newly forked individually |
| 2 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | [benyamin-persia/last30days-skill](https://github.com/benyamin-persia/last30days-skill) | Already existed; verified |
| 3 | [dream-num/univer](https://github.com/dream-num/univer) | [benyamin-persia/univer](https://github.com/benyamin-persia/univer) | Newly forked individually |
| 4 | [elementalsouls/Claude-BugHunter](https://github.com/elementalsouls/Claude-BugHunter) | [benyamin-persia/Claude-BugHunter](https://github.com/benyamin-persia/Claude-BugHunter) | Newly forked individually |
| 5 | [kajisho5/ffmpeg-skill](https://github.com/kajisho5/ffmpeg-skill) | [benyamin-persia/ffmpeg-skill](https://github.com/benyamin-persia/ffmpeg-skill) | Already existed; verified |

### Additional recent sources and outcomes

- [AKhomssi's Diagram Design post](https://x.com/AKhomssi/status/2126067216286167234) cross-referenced the earlier [Suraj Sharma ten-repository collection](10-ai-workflow-repositories-suraj/README.md). The source project [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) has a verified personal fork at [benyamin-persia/diagram-design](https://github.com/benyamin-persia/diagram-design). Commit `3cb4d80`.
- [0xCarnagee's X article](https://x.com/i/article/2125987874793226240) about model prompting/refusal behavior was cataloged at [`model-jailbreak-guide-carnage/README.md`](model-jailbreak-guide-carnage/README.md). It does not link a GitHub repository to fork; the page attributes and summarizes it rather than reproducing bypass instructions. Commit `28f9127`.
- [de1lymoon's Gemini Neon prompt post](https://x.com/de1lymoon/status/2126023253324079232) was cataloged at [`gemini-neon-system-prompt-de1lymoon/README.md`](gemini-neon-system-prompt-de1lymoon/README.md). It describes seven advertised modes/playbooks; performance claims are marked unverified. No GitHub repo was linked. Commit `e808321`.
- [CrazyShyyt's MeMo post](https://x.com/CrazyShyyt/status/2125859848965534161) led to [`memo-memory-as-model/README.md`](memo-memory-as-model/README.md), documenting the [MeMo paper](https://arxiv.org/abs/2605.15156), upstream implementation [arunv3rma/MeMo](https://github.com/arunv3rma/MeMo), and verified personal fork [benyamin-persia/MeMo](https://github.com/benyamin-persia/MeMo). The note preserves benchmark-scope and training-cost caveats rather than repeating “RAG is dead” as a fact. Commit `487c4a5`.
- [27_bishal's model post](https://x.com/27_bishal/status/2125830912453779582) was expanded into [`27-bishal-image-models/README.md`](27-bishal-image-models/README.md), with ten individual Hugging Face checkpoint/LoRA links. One entry, [Qwen-Image-2.1-Uncensored-Omni-Quantized](https://huggingface.co/chatrlabs/Qwen-Image-2.1-Uncensored-Omni-Quantized), was already cataloged. These are model pages, not GitHub projects to fork. Commit `3fd61c1`.
- [HShaabani's LightVela post](https://x.com/HShaabani/status/2125754893172699233) was cataloged at [`lightvela/README.md`](lightvela/README.md), along with the [official site](https://lightvela.ai/), [overview docs](https://lightvela.ai/docs/overview), [subscription page](https://lightvela.ai/subscribe), and [privacy policy](https://lightvela.ai/privacy-policy). It is a hosted service, not a GitHub repo to fork. Commit `f557292`.
- [ai_ba_reza's Nodaroo post](https://x.com/ai_ba_reza/status/2125866383414280647) was cataloged at [`nodaroo-free-hosting/README.md`](nodaroo-free-hosting/README.md), with the [invite page](https://free.nodaroo.com/invite/K3CbWxqIGwTj9XfrHc8wlA). The page recorded that free-server creation was closed when checked, despite the post's free-hosting claims. No GitHub repo to fork. Commit `fc0f736`.
- [The_MissAI's uncensored-model directory post](https://x.com/The_MissAI/status/2126065549096489402) was cataloged at [`free-uncensored-models-tools-k2s/README.md`](free-uncensored-models-tools-k2s/README.md), pointing to [K2S's directory](https://freeuncensoredaimodel.vercel.app). The directory covers five model picks and five tools/services. Five GitHub projects were individually checked: [p-e-w/heretic](https://github.com/p-e-w/heretic) → [your Heretic fork](https://github.com/benyamin-persia/heretic) (already existed); [ggml-org/llama.cpp](https://github.com/ggml-org/llama.cpp) → [your llama.cpp fork](https://github.com/benyamin-persia/llama.cpp) (already existed); [elder-plinius/OBLITERATUS](https://github.com/elder-plinius/OBLITERATUS) → [your OBLITERATUS fork](https://github.com/benyamin-persia/OBLITERATUS) (already existed); [PurpleDoubleD/locally-uncensored](https://github.com/PurpleDoubleD/locally-uncensored) → [your fork](https://github.com/benyamin-persia/locally-uncensored) (new); and [techjarves/Uncensored-Local-AI-Multiplatform](https://github.com/techjarves/Uncensored-Local-AI-Multiplatform) → [your fork](https://github.com/benyamin-persia/Uncensored-Local-AI-Multiplatform) (new). Commit `09617a2`.
- [Code Cloud's MotionSites MCP post](https://x.com/codecloude/status/2126063183064351094) was added at [`motionsites-mcp/README.md`](motionsites-mcp/README.md), with [MotionSites MCP](https://motionsites.ai/mcp) and its [MCP endpoint](https://motionsites.ai/api/mcp). This is a hosted connector with a limited free tier and paid library access, not a GitHub repo. Commit `6724b20`.
- [ToPassTheTimee's Orca post](https://x.com/ToPassTheTimee/status/2125998021334736948): upstream [stablyai/orca](https://github.com/stablyai/orca) → newly created, parent-verified [benyamin-persia/orca](https://github.com/benyamin-persia/orca). Catalog: [`orca/README.md`](orca/README.md). Commit `dcc23bc`.
- [mu4to's QuickOCR post](https://x.com/mu4to/status/2126001339196907836): upstream [Abolfazlshahi/QuickOCR](https://github.com/Abolfazlshahi/QuickOCR) → newly created, parent-verified [benyamin-persia/QuickOCR](https://github.com/benyamin-persia/QuickOCR). Catalog: [`quickocr/README.md`](quickocr/README.md). Its application source is MIT; bundled OCRia-nano weights have separate licensing. Commit `49d6e94`.
- [hsianghui's Blender Skills post](https://x.com/hsianghui/status/2125945423508762903): upstream [arjun988/blender-skills](https://github.com/arjun988/blender-skills) → previously existing, parent-verified [benyamin-persia/blender-skills](https://github.com/benyamin-persia/blender-skills). Catalog: [`blender-skills/README.md`](blender-skills/README.md). Commit `4210de1`.
- [Code Cloud's five-site/book list](https://x.com/codecloude/status/2125520261852065854) and [The_MissAI's seven-book-sites post](https://x.com/The_MissAI/status/2125448358743388660), along with the earlier post, have their own catalog entries; see [`7-free-book-sites-methcode/README.md`](7-free-book-sites-methcode/README.md) and the main README's Website Collections section. These pages are websites, not repositories to fork.

## Broader catalog already in place

The items above are the newest portion, not the whole project. The current main [`README.md`](README.md) is the complete category index. It links earlier work including, among others:

- X/tutorial-driven GitHub collections: [10 AI Workflow Repositories](10-ai-workflow-repositories-suraj/README.md), [50 Useful GitHub Repositories](50-useful-github-repositories-taqimolavi/README.md), [7 Open-Source Work Automation Projects](7-open-source-work-automation/README.md), [7 GitHub Repos for Designers](7-github-repos-for-designers/README.md), [19 AI Agent Ecosystem](19-ai-agent-ecosystem/README.md), [10 Fable Repositories](10-fable-52-repositories/README.md), [12 Motion/Video Repositories](12-motion-video-repositories/README.md), [11 Research-to-Video Repositories](11-research-to-video-workflow/README.md), [14 AI Video Production Repositories](14-ai-video-production/README.md), [18 AI Design Links](18-ai-design-links-bardhyl/README.md), and [8 AI Design Websites](8-ai-design-websites/README.md).
- Individual projects and resources across agent frameworks, skills, reverse engineering, voice/audio, UI, video, model research/local inference, and desktop utilities. Their detail pages are linked in the main README and retain the source URLs and fork pairs.
- Website/model/learning directories that are not GitHub repositories are deliberately cataloged without inventing forks. Examples include [50 Useful Websites](50-useful-websites/README.md), [Methcode's 50 Websites](methcode-50-websites/README.md), [Claude Skills Library](skillsclau.de/README.md), [AI company learning resources](ai-company-learning-resources/README.md), and the model pages in the AI Model Platforms category.

When an old item appears again in a new post, preserve the new attribution by adding a cross-reference in the existing detail page or appropriate collection. Avoid making duplicate catalog entries or duplicate GitHub forks just because an item was reshared.

## Current repository state at the time this file was written

The branch was `main`, tracking `origin/main`, and the worktree was clean before this file was added. The latest recorded commit was `e2b5e1e` (`Catalog Carrera's animation repositories`). The commit sequence immediately before this handoff includes the recent additions and updates listed above. After this file is committed and pushed, update this paragraph if future work makes it stale.

## Reusable prompt for the next ChatGPT session

Copy this prompt and replace the bracketed URL with the new URL. The repository rules below are intentionally explicit because the user expects the linked projects to be forked individually, not only collected into a list.

```text
I maintain https://github.com/benyamin-persia/ai-resources. Process this new source: [PASTE THE URL HERE].

This is an ongoing workflow. First inspect the existing repository, especially README.md and WORKFLOW_AND_HANDOFF.md, so you continue the established catalog and do not duplicate work. I expect you to do the work, not merely suggest what I could do.

For the supplied source:
1. Open and inspect it. Extract every distinct resource it actually links to, in the original order and categories. If the page is inaccessible, say exactly what could and could not be verified; do not invent its contents.
2. Investigate each item individually. Record its canonical source link, a short accurate description, and any important license, cost/access, hardware, privacy, safety, or reliability caveats. Attribute claims that come only from the post.
3. For EVERY GitHub repository in the source, check whether my account already has the correct fork. My account is https://github.com/benyamin-persia. Verify the fork's parent relationship to the upstream; matching names alone do not count. If a correct fork exists, link it and mark it as pre-existing. If it does not, create that repository as an individual fork of that exact upstream, then verify the parent metadata. Do this separately for every missing repo—do not skip entries, do not just create a combined repo, and do not call something a fork unless GitHub confirms the relationship. Never create duplicate forks if the correct one already exists.
4. Do not try to fork websites, X posts, articles, Hugging Face models, videos, hosted services, or other non-GitHub resources. Catalog them with their real canonical links instead. If an item links to a GitHub repository indirectly, explain that provenance.
5. Add a dedicated, readable Markdown detail page for the source/list, preserving the original sequence and showing each upstream -> my fork pair. Cross-reference existing entries and preserve new attribution when an item is a repeat. Add/update the appropriate category in README.md. Keep the catalog descriptive; do not copy large copyrighted content or unsafe instructions.
6. Check all changed files and links as practical, run `git diff --check`, and review the diff. Commit and push the completed changes to the existing origin/main if repository authentication is available. Do not claim a fork, commit, or push succeeded unless verified. If blocked, finish all safe catalog work and report the exact remaining item(s).
7. In your final report, give the source URL, the catalog file, the number of distinct GitHub repositories, how many forks were already there versus individually created now, any non-GitHub items, caveats/blockers, and the commit/push result. Be direct and thorough.

My requirement: “fork every repo one by one” means individually verify and fork every distinct GitHub upstream that lacks the correct fork in my account. It does not mean one umbrella repository or merely listing upstream URLs.
```

## Simple rule for future sessions

Take each URL seriously, investigate it, preserve what it actually points to, fork each missing GitHub repo individually, update the categorized catalog, verify the work, and clearly report what happened. The latest source is not necessarily a replacement for older work; add it to this continuing library.
