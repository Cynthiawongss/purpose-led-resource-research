# Research and Select Resources for a Specific Purpose

[简体中文](README.zh-CN.md) · [Install](docs/INSTALL.md) · [Worked example](examples/subtitle-selection.en.md) · [Validation](validation/README.md)

**Find resources that fit the task, explain why they fit, and show what remains uncertain.**

![A purpose branches into candidate sources; evidence and constraints guide a traceable shortlist. Check marks mean support in the supplied material, not runtime verification.](assets/hero.png)

*Purpose → source and condition checks → a traceable choice. A check mark means documented support, not a runtime test.*

An instruction-based Codex skill for comparing software, open-source projects, assets and documentation. It starts with purpose and constraints, then checks available content, conditions and evidence. The host supplies search and file-reading capabilities.

## What it changes

| Candidate claim | The follow-up question |
|---|---|
| Free subtitle tool | Is the required export free too? |
| Supports Mac | Which chip and system version? |
| Runs locally | Do both the video and recognition remain local? |
| Supports bilingual subtitles | Two languages in one SRT, or two separate files? |
| Open source | What is actually available, and under what conditions? |

## A concrete result

**Request:** Process private demo videos on an Apple Silicon Mac and export Chinese-English bilingual SRT for free, locally, using only supplied evidence.

All candidates here are fictional, not real product recommendations.

| Candidate | Decision | Reason |
|---|---|---|
| WindowCaption | Conditional documentation-based choice, not tested | Confirm macOS 13+; requires a 1.8 GB model download |
| NimbusSub | Excluded | Uploads original video |
| VerseDesk | Excluded | SRT export requires payment |
| MonoFrame | Excluded as supplied | Separate single-language files, no complete bilingual workflow supplied |
| ShellSRT | Pending information | Mac support, provider location and fees unclear |

The README and export documentation for one project remain one candidate with multiple evidence links. If nothing fits, report the gap instead of filling a quota.

[Read the full before/after example →](examples/subtitle-selection.en.md)

## Install

Send this in Codex:

~~~text
Use skill-installer to install the skill from:
https://github.com/cynthiawongss/purpose-led-resource-research/tree/main/skills/purpose-led-resource-research
~~~

Or download an English or Chinese skill ZIP from the [v0.1.0 release](https://github.com/cynthiawongss/purpose-led-resource-research/releases/tag/v0.1.0). Install one language variant only. [Manual setup and updates →](docs/INSTALL.md)

## Use it

Describe the task naturally:

> Compare Mac screen recorders for recording system audio and exporting without watermarks. Explain costs, sources and uncertainties.

For explicit selection:

~~~text
Use $purpose-led-resource-research to compare these candidates against my
mandatory requirements. Preserve sources and separate documented claims
from runtime testing.
~~~

Automatic matching depends on the host and task description. English instructions can serve Chinese requests and vice versa; [complete Chinese instructions](docs/SKILL.zh-CN.md) are also available. See [OpenAI's skill documentation](https://learn.chatgpt.com/docs/build-skills) for discovery and invocation.

## Scope and limits

- Useful for resource research, comparison and selection; not needed for translation, summarization or reorganizing an existing collection alone.
- No bundled search provider, account, API or required Agent Reach dependency. Live research needs host capabilities.
- A documentation-supported recommendation is not a runtime verification. A research request does not authorize installation, purchases or signup.
- Missing, stale or inaccessible evidence stays uncertain. A fitting option may not exist.

**Version 0.1.0 — early public release.** English and Chinese offline simulated trials are documented. Live research quality, automatic invocation and cross-model stability are not established. [Validation scope →](validation/README.md)

## Companion skill

Already have the materials, but cannot understand the categories, fields or relationships? See [Classify and Restructure Complex Materials](https://github.com/cynthiawongss/restructure-complex-materials).

## Origin and contributions

Distilled from the author's resource-research practice with Codex assistance in drafting, translation and validation. To report a problem, provide a synthetic or redacted input, the expected behavior and the actual result.

[MIT License](LICENSE) · [Method and image provenance](docs/PROVENANCE.md)
