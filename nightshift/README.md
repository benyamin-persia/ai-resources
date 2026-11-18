# Nightshift

Shared in [HazratCrypto's X post](https://x.com/HazratCrypto/status/2122824376013717829), which recommends queued overnight coding work with a per-item morning receipt.

- Upstream: [orwa-mahmoud/nightshift](https://github.com/orwa-mahmoud/nightshift)
- Your individual fork: [benyamin-persia/nightshift](https://github.com/benyamin-persia/nightshift)
- License shown by upstream: MIT.

The upstream README describes Nightshift as a plugin for Claude Code, Codex, and Cursor. It supports planning a punch list, running items as a shift, and reviewing per-item receipts that record delivered work, attempted/rejected approaches, checks, evidence, duration, and token usage. The README currently lists 32 ready-made shifts. The post's “458 stars” figure is a point-in-time claim and will change; GitHub displayed a different count when this collection was checked.

The post correctly cautions that Git history alone does not prove code is correct. Nightshift provides receipts/check evidence, but a human still needs to review the changes and judge whether the tests and evidence are adequate. Before installing, review the plugin's hooks/permissions and use an appropriate isolated branch or worktree for unattended changes.

The repository describes setup and commands for each supported host in its [upstream README](https://github.com/orwa-mahmoud/nightshift#install).
