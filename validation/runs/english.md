# English execution — fictional resource-selection packet

Review date: 2026-11-20. This answer uses only the supplied synthetic excerpts S1–S6. The linked `.invalid` addresses identify fictional sources; they were not opened. No software was installed or executed, and no real product capabilities were verified.

## First request

**Choose WindowCaption on the supplied documentation, provided your Mac runs macOS 13 or later.** S1 and S2 together support Apple Silicon, on-device video/audio processing, a free local workflow, and one SRT containing both Chinese and English lines. The 1.8 GB model download is compatible with your stated allowance. This is a recommendation supported by supplied documentation, not a runtime-tested result. Your OS version was not supplied, so machine-specific compatibility remains to be confirmed.

The mandatory conditions are Apple Silicon compatibility, original-video processing on the device, Chinese-English bilingual SRT export, and no charge anywhere in that workflow. A separate model download is allowed. Prior runtime testing is not required. I interpret bilingual SRT as both languages in one SRT file, consistent with S1 and the explicit limitation described in S5.

| Resource and available material | Mandatory-condition assessment | Decision and limitations | Evidence |
|---|---|---|---|
| **WindowCaption** — one project represented by a README and export/usage documentation | Apple Silicon and macOS 13+; all video/audio processing on-device; Chinese and English lines in one SRT; local inference and bilingual export free, with no account, credits, or API key | **Documentation-supported choice**, conditional on macOS 13+. Download the 1.8 GB model before first use. Optional paid collaboration is unnecessary for this workflow. Subtitle accuracy and successful operation have not been tested. | [S1: README](https://windowcaption.invalid/repo), [S2: export documentation](https://windowcaption.invalid/docs/export); supplied excerpts only |
| **NimbusSub** — browser product described by a product page | Browser use on Mac and bilingual subtitles/SRT claimed; video must be uploaded to its server | **Excluded:** required upload violates local original-video processing. Free registration does not establish that the whole export workflow is free. Apple Silicon-specific support and the precise bilingual layout in the SRT are not separately established. | [S3: product page](https://nimbussub.invalid); supplied excerpt only |
| **VerseDesk** — native app described by pricing/platform notes | Apple Silicon and private local processing stated; every SRT export, including bilingual, requires Pro | **Excluded:** mandatory SRT export is paid. Free basic editing does not satisfy the end-to-end cost requirement. | [S4: pricing/platform notes](https://versedesk.invalid/pricing); supplied excerpt only |
| **MonoFrame** — tool described by an export specification | Apple Silicon, local processing, and no fees stated; only one language per SRT, with Chinese and English available as separate files | **Excluded as a complete solution:** no built-in bilingual SRT export. The packet supplies no supported additional tool or merging workflow, so two monolingual files cannot be treated as fulfilling the requested output. | [S5: export specification](https://monoframe.invalid/export); supplied excerpt only |
| **ShellSRT** — repository-based setup, not an established ready-to-use Mac app | Local Linux setup and bilingual SRT stated; speech recognition depends on a separately configured provider | **Pending verification, not qualified:** Apple Silicon/macOS compatibility, provider location and end-to-end charges are unknown. “Run locally” does not establish that the recognition provider processes locally. License terms also absent. | [S6: repository instructions](https://shellsrt.invalid/readme); supplied excerpt only |

WindowCaption’s README and export documentation are two entry points for the same project, not two recommendations. The excerpts establish claims about functionality and cost; they do not establish source-code availability or an open-source license. Open-source licensing is not one of your mandatory conditions.

### What to check next

1. Confirm your installed macOS version is at least 13 and that you have room for the 1.8 GB model plus video and output files. The packet supplies no memory or additional storage requirement.
2. Use S1 as the setup entry point and S2 to identify local inference and bilingual SRT export. Confirm the local mode does not require enabling the optional hosted collaboration workspace. No account or purchase should be needed according to S2.
3. When you choose to run a trial, use a short, non-sensitive sample first. Check that the model is available locally, original media processing remains on-device, both Chinese and English appear in each appropriate subtitle cue in the exported SRT, timing and text are usable, and no payment or API configuration is required. This is a proposed check, not something performed here. Translation quality and runtime reliability remain untested.

There is no need to install or run anything to receive the present recommendation. These next steps describe how to validate it later; this answer has stayed within your packet-only research scope.

### Requirement-to-source audit

| Required field | Supplied value used for the choice | Source and evidence gap |
|---|---|---|
| Platform | macOS 13+, Apple Silicon | S1; your installed OS version unknown |
| Data location | All video and audio processing on-device | S1; excerpt claim, no execution or network observation |
| Preparation | Download a 1.8 GB speech model before first run | S1; separate download explicitly acceptable in your request |
| Output format and languages | Chinese and English lines in one SRT | S1; actual exported file not inspected |
| Complete-workflow cost | Local inference and bilingual SRT export free; no account, credits or API key | S2; no runtime log supplied |
| Optional service cost | Hosted collaboration subscription, unnecessary for local export | S2; not included in proposed workflow |
| Alternative failures and unknowns | Required upload; paid SRT; separate monolingual SRTs; undocumented Mac/provider conditions | S3; S4; S5; S6, respectively, as detailed above |

## Separate follow-up: only S3–S6 available

**I cannot recommend a qualified solution from this reduced packet under the unchanged requirements.** This does not establish that no such tool exists; it means the remaining evidence does not support one.

- **NimbusSub (S3)** requires uploading the original video to a server and therefore fails the privacy condition. A free account also does not demonstrate free completion.
- **VerseDesk (S4)** requires payment for SRT export and therefore fails the free-workflow condition.
- **MonoFrame (S5)** cannot export a bilingual SRT directly. It provides two separate monolingual files, and the packet provides no verified way to produce the required combined file for free while keeping processing local.
- **ShellSRT (S6)** remains a verification lead only. Its Linux instructions do not establish macOS/Apple Silicon compatibility, and the separately configured recognition provider’s location and charges are unknown. Bilingual SRT support alone is insufficient.

For a next research step, request documentation covering ShellSRT’s supported Apple Silicon installation, its complete recognition and bilingual-processing path, where every relevant processing stage occurs, and all provider/export costs. Check license terms as well before use. Alternatively, obtain documentation for a complete free local bilingual-export workflow; any proposed addition to MonoFrame would need its own compatibility, privacy, cost and output evidence. None of those additions is supplied or verified here. Until that evidence exists, keep the choice unresolved rather than accepting upload, payment, or separate monolingual exports.
