# NVIDIA Auto Ontology

Shared in [Shoumya23's X post](https://x.com/Shoumya23/status/2126520875377959191). The post links one GitHub project: [NVIDIA/auto-ontology](https://github.com/NVIDIA/auto-ontology).

## What it is

Auto Ontology is an Apache-2.0 Python framework for generating and maintaining a semantic layer over enterprise data. Its ontology represents business concepts, mappings to database columns, relationships/joins, metric definitions, lineage, and certification status. The goal is to give analytics agents explicit, reviewable business context so they can map natural-language questions to data and produce SQL with an explanation.

The upstream project describes workflows to discover an ontology from database metadata, ground agent questions in its concepts and relationships, validate the result with questions, and expose context through MCP, CLI, and API. It is intended to complement existing semantic models and supports the portable [Apache Ossie](https://ossie.apache.org/) ontology format.

## Upstream and your fork

| Upstream | Your individual fork | Fork status |
|---|---|---|
| [NVIDIA/auto-ontology](https://github.com/NVIDIA/auto-ontology) | [benyamin-persia/auto-ontology](https://github.com/benyamin-persia/auto-ontology) | Already existed; GitHub confirms the fork parent is `NVIDIA/auto-ontology` |

No new fork was needed for this post. The source is a GitHub repository, and the personal fork relationship was checked directly rather than inferred from the repository name.

## Setup and practical notes

The upstream quickstart uses Docker Compose with PostgreSQL and pgvector, `uv`, and an NVIDIA API key. The example launches a Wide World Importers sample database and a local web application; the README also documents MCP/CLI/API integration. This is therefore a full data/agent stack, not a lightweight single-command library install.

Before running it, configure unique passwords and secrets in `.env`, keep API keys private, and avoid exposing the sample database or management services to untrusted networks. Use only data you are authorized to process; review how database metadata, query history, PII detection, and model-provider requests are configured for your environment.

The upstream README advertises top results on the BEAVER and BIRD-Interact benchmarks. Treat leaderboard statements and performance claims as project-reported and check the linked benchmark methodology and current results before relying on them. The project itself notes that a semantic ontology is most valuable for ambiguous questions over large, messy, or conflicting data; simple, well-modeled data with fixed questions may not need this layer.

## Links

- Original post: [Shoumya23 on X](https://x.com/Shoumya23/status/2126520875377959191)
- Upstream repository and documentation: [NVIDIA/auto-ontology](https://github.com/NVIDIA/auto-ontology)
- Your fork: [benyamin-persia/auto-ontology](https://github.com/benyamin-persia/auto-ontology)
- [BEAVER benchmark](https://beaverbench.github.io/)
- [BIRD-Interact benchmark](https://bird-interact.github.io/)
- [Apache Ossie](https://ossie.apache.org/)
