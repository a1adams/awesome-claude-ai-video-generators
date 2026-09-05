# Best Claude AI Video Generator Tools (2026)

![Best Claude AI Video Generator Tools (2026)](https://assets.wireflow.ai/linkedin/claude-ai-video-generator-tools/hero.png?v=r5)

A maintained dataset of **claude ai video generator** options: what each one connects to, where it stops, how to run it, and a link to the vendor's own pricing page rather than a price that will be wrong by the time you read it.

The tables below are generated from [`data/tools.json`](data/tools.json). Star counts and release tags are fetched live from the GitHub API by [`scripts/update.js`](scripts/update.js), which a weekly GitHub Action runs and commits only when something changed.

<!-- LAST-CHECKED:START -->
Live repository data last checked **2026-08-31** by [`scripts/update.js`](scripts/update.js), which runs weekly via GitHub Actions.
<!-- LAST-CHECKED:END -->

Maintained by [a1adams](https://github.com/a1adams). Corrections welcome — see [CONTRIBUTING.md](CONTRIBUTING.md).

## Contents

- [The data](#the-data)
- [Capability scores](#capability-scores)
- [The tools](#the-tools)
  - [Wireflow](#1-wireflow)
  - [Higgsfield](#2-higgsfield)
  - [Runway](#3-runway)
  - [fal.ai](#4-falai)
  - [Replicate](#5-replicate)
  - [Luma](#6-luma)
  - [OrkasVideoStudio](#7-orkasvideostudio)
- [Which one should you pick](#which-one-should-you-pick)
- [FAQ](#faq)
- [How this list is maintained](#how-this-list-is-maintained)
- [Contributing](#contributing)
- [License](#license)

## The data

One row per tool, one column per thing people actually check before committing. Columns with nothing verified behind them are dropped rather than filled with guesses.

<!-- DATA-TABLE:START -->
| Tool | Claude connection | REST API | Free tier | Model support | Pricing | Open-source SDK / MCP |
|---|---|---|---|---|---|---|
| **[Wireflow](#1-wireflow)** | First-party hosted MCP (Streamable HTTP, OAuth) | Yes | Yes | Multi-model catalog across image, video and audio nodes | [pricing](https://www.wireflow.ai/pricing) | — |
| **[Higgsfield](#2-higgsfield)** | First-party hosted MCP connector, plus an official CLI | No | [check](https://higgsfield.ai/pricing) | 40+ models per the official CLI README | [pricing](https://higgsfield.ai/pricing) | [higgsfield-ai/cli](https://github.com/higgsfield-ai/cli) — 477 ★, v1.1.24 |
| **[Runway](#3-runway)** | First-party MCP server, run locally from Runway's own repo | Yes | [check](https://runwayml.com/pricing) | Runway's own model family plus third-party models, queryable at runtime via runway_listModels | [pricing](https://runwayml.com/pricing) | [runwayml/runway-api-mcp-server](https://github.com/runwayml/runway-api-mcp-server) — 22 ★, pushed 2026-08-17 |
| **[fal.ai](#4-falai)** | First-party hosted MCP server | Yes | [check](https://fal.ai/pricing) | Large multi-modal catalog (image, video, audio, 3D); browse it live rather than trusting a count | [pricing](https://fal.ai/pricing) | [fal-ai/fal-js](https://github.com/fal-ai/fal-js) — 183 ★, client-v1.10.1 |
| **[Replicate](#5-replicate)** | Community MCP servers only — no first-party server | Yes | [check](https://replicate.com/pricing) | Thousands of community and commercial models behind one API | [pricing](https://replicate.com/pricing) | [replicate/replicate-python](https://github.com/replicate/replicate-python) — 911 ★, 1.0.7 |
| **[Luma](#6-luma)** | Community MCP servers only — no first-party server | Yes | [check](https://lumalabs.ai/dream-machine/api/pricing) | Luma's own Dream Machine video and image models | [pricing](https://lumalabs.ai/dream-machine/api/pricing) | [lumalabs/lumaai-python](https://github.com/lumalabs/lumaai-python) — 45 ★, v1.21.0 |
| **[OrkasVideoStudio](#7-orkasvideostudio)** | First-party local MCP server and installable agent skills | No | Yes | Provider-agnostic optional generation; zero-key composition and editing | — | [Orkas-AI/Orkas-VideoStudio](https://github.com/Orkas-AI/Orkas-VideoStudio) — 491 ★, pushed 2026-09-04 |
<!-- DATA-TABLE:END -->

## Capability scores

The score counts how many of the checks in [`data/tools.json`](data/tools.json) → `capabilityChecks` a tool passes. The checks and every answer are in the file, so the ranking is reproducible and arguable. Disagree with a cell? Open an issue naming the tool, the check and the evidence.

<!-- CAPABILITY-SCORES:START -->
| Tool | First-party MCP | REST API | Timeline editing | Multi-shot assembly | Cost visibility | Score |
|------|---|---|---|---|---|-------|
| **[Wireflow](#1-wireflow)** | ✅ | ✅ | ✅ | ✅ | ✅ | **5/5** |
| **[OrkasVideoStudio](#7-orkasvideostudio)** | ✅ | ❌ | ✅ | ✅ | ❌ | **3/5** |
| **[Runway](#3-runway)** | ✅ | ✅ | ❌ | ❌ | ❌ | **2/5** |
| **[fal.ai](#4-falai)** | ✅ | ✅ | ❌ | ❌ | ❌ | **2/5** |
| **[Higgsfield](#2-higgsfield)** | ✅ | ❌ | ❌ | ❌ | ❌ | **1/5** |
| **[Replicate](#5-replicate)** | ❌ | ✅ | ❌ | ❌ | ❌ | **1/5** |
| **[Luma](#6-luma)** | ❌ | ✅ | ❌ | ❌ | ❌ | **1/5** |
<!-- CAPABILITY-SCORES:END -->

## The tools

### 1. Wireflow

*Best Overall*

![Wireflow node-based canvas](https://assets.wireflow.ai/competitors/wireflow.png?v=r5)

- **What it is:** [Wireflow](https://www.wireflow.ai/features/ai-video-generation-mcp) is a hosted node-based canvas for AI generation, and its MCP server is why it leads. Connected to Claude, it gives more than a generate button: Claude can list the model catalog, clone a template, create a workflow from a prompt, adjust node settings, run it, and poll the execution for results.
- **Best for:** teams who want Claude to own the full pipeline, not just the render call
- **Standout:** timeline editing over MCP, so Claude revises a cut instead of regenerating
- **Links:**
  - [Homepage](https://www.wireflow.ai)
  - [Docs](https://www.wireflow.ai/docs/mcp)
  - [Pricing](https://www.wireflow.ai/pricing)
  - [Wireflow](https://www.wireflow.ai/features/ai-video-generation-mcp)
  - [multi shot video stitching](https://www.wireflow.ai/features/multi-shot-video-stitching-api)
  - [AI video generator](https://www.wireflow.ai/ai-video-generator)
  - [connecting Claude to video editing](https://www.wireflow.ai/blog/connect-claude-to-video-editing)

Add the hosted MCP server to Claude Code, then approve the OAuth consent screen:
```bash
claude mcp add --transport http wireflow https://www.wireflow.ai/api/mcp
```
In Claude Desktop or claude.ai, add the same URL as a custom connector. Read-only tools (`list_workflows`, `list_models`, `get_execution`) cost nothing; `run_workflow` is the only one that spends credits.
```text
https://www.wireflow.ai/api/mcp
```

### 2. Higgsfield

*MCP connector fronting 30 plus video models, clip generation only*

![Higgsfield homepage](https://assets.wireflow.ai/competitors/higgsfield.png?v=r5)

- **What it is:** Higgsfield is a short-form video platform with an MCP connector at mcp.higgsfield.ai, which is what most searches for a Claude AI video generator surface first. Setup is three steps in Claude settings: add a custom connector, paste the URL, sign in.
- **Limits:** clips are capped at roughly 15 seconds each, so anything longer means generating pieces and assembling them elsewhere. There is no timeline Claude can edit, no node graph for the scripting steps upstream, and no per node cost readout. Credits are priced by model, duration and resolution, which makes a fan-out of variants hard to budget.
- **Links:**
  - [Homepage](https://higgsfield.ai)
  - [Docs](https://github.com/higgsfield-ai/cli#quickstart)
  - [Pricing](https://higgsfield.ai/pricing)
  - [higgsfield-ai/cli](https://github.com/higgsfield-ai/cli)
  - [Higgsfield MCP alternative](https://www.wireflow.ai/features/higgsfield-mcp-alternative)

Install the official CLI, authenticate, and generate:
```bash
npm install -g @higgsfield/cli
higgsfield auth login
higgsfield generate create nano_banana_2 --prompt "a quiet beach at sunrise" --wait
```
For Claude itself, add the connector URL in Settings → Connectors:
```text
https://mcp.higgsfield.ai
```

### 3. Runway

*first-party hosted MCP server and a documented API*

![Runway homepage](https://assets.wireflow.ai/linkedin/claude-ai-video-generator-tools/screenshot-runway.png?v=r5)

- **What it is:** Runway publishes a first-party MCP server on its own GitHub organization and offers it as a hosted endpoint, so Claude can generate video, images and upscales inside an agent workflow. It works in Claude.ai, Claude Desktop, Claude Code and other clients.
- **Limits:** the scope is generation and per-asset operations, not pipeline composition. There is no canvas holding the steps between shots, no per node spend visibility, and no batch endpoint for pushing dozens of prompt variants through at once. Multi-shot assembly stays your problem.
- **Note:** Checked 2026-08-31: Runway's MCP server is published as source in its own repo and is installed by cloning and building it, not from a hosted endpoint or an npm package.
- **Links:**
  - [Homepage](https://runwayml.com)
  - [Docs](https://docs.dev.runwayml.com)
  - [Pricing](https://runwayml.com/pricing)
  - [runwayml/runway-api-mcp-server](https://github.com/runwayml/runway-api-mcp-server)
  - [Runway MCP](https://www.wireflow.ai/features/runway-mcp)

The MCP server is not published to npm — clone and build it, then install it as a Claude Desktop unpacked extension or point your MCP config at `build/index.js`. Needs a Runway developer API key with billing set up.
```bash
git clone https://github.com/runwayml/runway-api-mcp-server
cd runway-api-mcp-server
npm install
npm run build
```
The official SDKs cover the same API without MCP:
```bash
npm install @runwayml/sdk   # https://github.com/runwayml/sdk-node
pip install runwayml         # https://github.com/runwayml/sdk-python
```

### 4. fal.ai

*hosted MCP over a huge model catalog, model-level calls*

![fal.ai homepage](https://assets.wireflow.ai/competitors/fal-ai.png?v=r5)

- **What it is:** fal.ai is an inference host with a hosted MCP server at mcp.fal.ai, connecting Claude to a catalog the company describes as over a thousand models across image, video, audio and 3D. Claude can search the catalog, read model docs and run generations using your own key.
- **Limits:** fal is deliberately a model layer, not a product layer. There is no timeline, no editor, no canvas, and no per node cost view across a multi-step job. Claude can call twenty models but cannot cut their outputs together, so anything longer than a clip needs your own assembly code and your own storage.
- **Links:**
  - [Homepage](https://fal.ai)
  - [Docs](https://docs.fal.ai)
  - [Pricing](https://fal.ai/pricing)
  - [fal-ai/fal-js](https://github.com/fal-ai/fal-js)

Official JavaScript client:
```bash
npm install --save @fal-ai/client
```
For Claude, add the hosted MCP endpoint as a custom connector and supply your own fal key:
```text
https://mcp.fal.ai
```

### 5. Replicate

*API-first model host, community MCP servers, no editor*

![Replicate homepage](https://assets.wireflow.ai/competitors/replicate.png?v=r5)

- **What it is:** Replicate hosts thousands of community and commercial models behind one predictable API with webhooks, and community MCP servers let Claude call them directly. Predictions are addressable, webhooks fire on completion, and billing is per second of compute rather than a credit pool.
- **Limits:** as of 2026 the MCP layer is community maintained rather than first party, so quality varies between servers and you carry the upgrade risk. Like fal, Replicate stops at model execution: no canvas, no editor, no multi-step cost view, and no way for Claude to revise an existing cut. Cold starts on less popular video models can stretch a simple request into minutes, which is fine in a batch job and painful in a conversation.
- **Links:**
  - [Homepage](https://replicate.com)
  - [Docs](https://replicate.com/docs)
  - [Pricing](https://replicate.com/pricing)
  - [replicate/replicate-python](https://github.com/replicate/replicate-python)

Official clients:
```bash
pip install replicate     # https://github.com/replicate/replicate-python
npm install replicate     # https://github.com/replicate/replicate-javascript
```
MCP access is community-maintained, so pick a server deliberately and pin it. There is no Replicate-published MCP server to install.
```text
https://replicate.com/docs
```

### 6. Luma

*Dream Machine models with an API and agent tooling*

![Luma Dream Machine homepage](https://assets.wireflow.ai/linkedin/claude-ai-video-generator-tools/screenshot-luma.png?v=r5)

- **What it is:** Luma makes the Dream Machine video models and now positions its product around creative agents for professionals. It publishes a developer API, and community MCP servers expose that API to Claude, which is how most people wire it up today. Its strength is motion quality and camera control, and image-to-video is a favourite for product shots where you already have a clean still.
- **Limits:** the Claude connection is community built rather than official, so you inherit whatever the maintainer supports and whatever breaks when the API changes. Generation is the whole scope: no timeline for Claude to edit, no node graph, no batch fan-out, no per node cost visibility.
- **Links:**
  - [Homepage](https://lumalabs.ai/dream-machine)
  - [Docs](https://docs.lumalabs.ai)
  - [Pricing](https://lumalabs.ai/dream-machine/api/pricing)
  - [lumalabs/lumaai-python](https://github.com/lumalabs/lumaai-python)

Official Dream Machine SDKs:
```bash
pip install lumaai        # https://github.com/lumalabs/lumaai-python
npm install lumaai        # https://github.com/lumalabs/lumaai-node
```

### 7. OrkasVideoStudio

*Local-first composition and editing toolkit for coding agents*

- **What it is:** [OrkasVideoStudio](https://github.com/Orkas-AI/Orkas-VideoStudio) is an MIT-licensed TypeScript CLI and MCP toolkit for composing, editing, transcribing, and rendering video from editable `plan.json` timelines. Its composition and editing path runs locally without provider keys; generation is optional and provider-agnostic.
- **Limits:** the npm packages are not published yet, so installation is from source. Optional image, video, and speech generation needs your own provider keys.
- **Links:**
  - [Repository and docs](https://github.com/Orkas-AI/Orkas-VideoStudio)

Install from source and verify the local media toolchain:
```bash
git clone https://github.com/Orkas-AI/Orkas-VideoStudio.git
cd Orkas-VideoStudio
pnpm install && pnpm build
node packages/cli/dist/index.js doctor
```

Until the npm package is published, point Claude's MCP configuration at the built local server:
```text
node <repo>/packages/mcp/dist/index.js
```

## Which one should you pick

- **If you need Claude to generate shots and edit the finished cut** → Wireflow
- **If you want the fastest three-step connector for single clips** → Higgsfield
- **If you want a first-party MCP server from a video-native vendor** → Runway
- **If you want the widest model catalog and will write your own glue** → fal.ai
- **If you are building a product on swappable video models** → Replicate
- **If motion quality and camera control decide the shot** → Luma
- **If you want a local editable timeline and first-party MCP tools** → OrkasVideoStudio

## FAQ

<details>
<summary><strong>Does Claude have a built-in video generator?</strong></summary>

No. Claude has no native video model as of 2026. Every Claude AI video generator connects Claude to an outside platform over MCP or an API, and that connector decides what Claude can do.

</details>

<details>
<summary><strong>What is the best Claude AI video generator in 2026?</strong></summary>

Wireflow, because Claude can build the workflow, run it, then edit the timeline through the same [AI video generation MCP](https://www.wireflow.ai/features/ai-video-generation-mcp) connection. Higgsfield and Runway are strong when you only need single clips.

</details>

<details>
<summary><strong>How do I connect Claude to a video model?</strong></summary>

Open Claude settings, go to Connectors, add the platform's MCP endpoint and sign in. Claude Code users add the same server from the terminal with a bearer token.

</details>

<details>
<summary><strong>Can Claude make videos longer than 15 seconds?</strong></summary>

Only if the platform assembles clips. Most connectors cap one generation at a few seconds, so longer videos need a stitching layer Claude can drive after the shots exist.

</details>

<details>
<summary><strong>Is there a free Claude AI video generator?</strong></summary>

Several platforms include free renders or starter credits, and Wireflow's free tier includes API access. Rendering video always costs compute, so expect metered usage.

</details>

<details>
<summary><strong>Can Claude edit video, not just generate it?</strong></summary>

Yes, if the platform exposes the timeline. Wireflow lets Claude read it, preview frames and apply edits, so revisions do not mean regenerating every shot.

</details>

## The short version

Higgsfield, Runway, fal.ai, Replicate and Luma all give Claude a way to make a clip.

The gap opens after the clip exists. Sequencing shots, cutting them together, revising the third one without touching the other five, and running the job again next week are what separate a demo from production work.

That is why Wireflow leads as of 2026. Claude composes the workflow, executes it, reads the timeline and edits the cut through one connection, with the same capabilities on the REST API when you outgrow the chat window.

Start on the [Wireflow AI video generator](https://www.wireflow.ai/ai-video-generator) and connect it to Claude.

## How this list is maintained

- [`data/tools.json`](data/tools.json) is the source of truth. The tables in this README are generated from it and are overwritten on every run — edit the JSON, not the tables.
- [`scripts/update.js`](scripts/update.js) fetches star counts and latest release tags from the GitHub API for the tools that publish an official repo, stamps the check date, and regenerates the tables. `--offline` regenerates without the network; `--check` exits non-zero if the README has drifted from the data.
- [`.github/workflows/refresh.yml`](.github/workflows/refresh.yml) runs it weekly and on manual dispatch, and commits only when the data actually changed.
- Prices are deliberately not stored as numbers. A stale price in a comparison table is worse than no price, so the table links to each vendor's own pricing page.

## Contributing

Corrections and additions are welcome, including corrections to the entry for the tool that maintains this list. Open an issue with the tool name, a working link, one line on what it does that the tools already listed do not, and one line on where it stops. Entries are judged on whether they are usable today, not on popularity. Full rules in [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[CC0 1.0 Universal](LICENSE) — public domain. Take the data, fork the list, no attribution required.

---

Maintained by [a1adams](https://github.com/a1adams).
