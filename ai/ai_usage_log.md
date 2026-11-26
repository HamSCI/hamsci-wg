# AI Usage Log: {{WORKING_GROUP_NAME}}

This log records every substantive AI-assisted session for the HamSCI working group
"{{WORKING_GROUP_NAME}}".

Required by the HamSCI Generative AI Use Agreement, and by any institutional or funder policy
that applies to this project (see `.claude/rules/ai-governance.md`).

**This log is the source of truth for what AI did on this project.** A disclosure paragraph in a
manuscript, poster, or software release summarizes this log truthfully. Keep it current: an
entry written from memory weeks later is not a record.

## Entry format

```
## [YYYY-MM-DD HH:MM TZ]
- **Tool**: Claude (Anthropic), <exact-model-id>
- **Session Purpose**: What the session set out to accomplish
- **Sections/Files Affected**: Specific files, sections, or documents touched
- **Nature of Contribution**: Draft / Edit / Analysis / Code generation / Research / Scaffolding
- **Human Review Status**: Reviewed and verified / Partially reviewed / Pending review
- **Git Hash**: <filled in after committing>
```

The date and time come from the system clock via `date`, never from an estimate. The `/commit`
command produces this format and appends it in the right order.

---

<!-- Append new entries below this line, newest at the bottom.
     On instantiating a new project from this template, delete every entry below:
     they belong to the template's own development, not to your project. -->

<!-- The first entry below was inherited from HamSCI/ai_project_template (commit ae4773a) when
     it was merged into hamsci-wg; its file paths refer to that repository's layout. -->

## [2026-09-22 20:43 UTC]
- **Tool**: Claude (Anthropic), claude-opus-5
- **Session Purpose**: Create the HamSCI `ai_project_template` by adapting
  `w2naf-academia/ai_project_template` for general HamSCI use: restructure the AI policy stack
  into three tiers so volunteer and student projects are not forced to carry institutional and
  funder sections, add HamSCI-specific rules for callsign attribution and station-location
  privacy, and add a getting-started onramp, LICENSE, CITATION.cff, and issue templates matching
  HamSCI house style.
- **Sections/Files Affected**: `README.md`, `CLAUDE.md`, `LICENSE`, `CITATION.cff`, `.gitignore`,
  `.claude/rules/ai-governance.md`, `.claude/rules/hamsci-data.md` (new),
  `.claude/rules/latex-writing.md`, `.claude/rules/python-code.md`, `.claude/commands/commit.md`,
  `.claude/settings.json`, `ai/ai_usage_log.md`, `docs/GETTING_STARTED.md`,
  `.github/ISSUE_TEMPLATE/` (bug_report, feature_request, question)
- **Nature of Contribution**: Scaffolding, drafting, and adaptation of an existing template
- **Human Review Status**: Pending review by N. A. Frissell (W2NAF)
- **Git Hash**: d1983ff

## [2026-09-26 13:32 UTC]
- **Tool**: Claude (Anthropic), claude-opus-5-5
- **Session Purpose**: Incorporate the contents of `HamSCI/ai_project_template` (commit
  `ae4773a`) into the `hamsci-wg` working-group website template on the `ai_project` branch,
  adapting it to the working-group layout: `docs/` is the published Jekyll site, so the
  getting-started guide moved to `ai/`, placeholder searches skip Liquid templates, and the
  README checklist, `CLAUDE.md`, and `CITATION.cff` were merged rather than replaced.
- **Sections/Files Affected**: `README.md`, `CLAUDE.md` (new), `CITATION.cff`, `LICENSE` (new),
  `.gitignore` (new), `.claude/` (new: `settings.json`, `commands/commit.md`,
  `rules/ai-governance.md`, `rules/hamsci-data.md`, `rules/latex-writing.md`,
  `rules/python-code.md`), `ai/ai_usage_log.md` (new), `ai/GETTING_STARTED.md` (new)
- **Nature of Contribution**: Scaffolding and adaptation of an existing template
- **Human Review Status**: Reviewed and verified by N. A. Frissell (W2NAF), 2026-09-26
- **Git Hash**: 49ba1f3

## [2026-11-14 15:09 UTC]
- **Tool**: Claude (Anthropic), claude-opus-5-5
- **Session Purpose**: Bring PR #3 up to date with `HamSCI/ai_project_template`, from `ae4773a` to
  `a09f960` (template PRs #1–#7): branch-then-PR workflow, AI log hash recorded on the change's
  own branch, the curated-documents rule, and the session-start template check with
  `/template-sync`. The template's changes were applied as changes, keeping the working-group
  adaptations (getting-started guide in `ai/`, the public-repository warning, the `src/README.md`
  note in the Python rule).
- **Sections/Files Affected**: `CLAUDE.md`, `README.md`, `.gitignore`, `.claude/settings.json`,
  `.claude/commands/commit.md`, `.claude/commands/template-sync.md` (new),
  `.claude/hooks/template_check.sh` (new), `.claude/template.json` (new, pinned at `a09f960`),
  `.claude/rules/ai-governance.md`, `.claude/rules/latex-writing.md`, `.claude/rules/python-code.md`,
  `ai/GETTING_STARTED.md`
- **Nature of Contribution**: Template sync and adaptation
- **Human Review Status**: Pending review by N. A. Frissell (W2NAF)
- **Git Hash**: 54b0204 (PR HamSCI/hamsci-wg#3)

## [2026-11-26 13:55 UTC]
- **Tool**: Claude (Anthropic), claude-opus-5-5
- **Session Purpose**: NAF: "All AI-opened PRs should be opened in Draft mode. A human will click to convert from draft mode to ready to merge." and "Give the user brief instructions to change the PR from draft to ready after they review. Also, be sure to give the URL to the user every time you create or modify a PR." Apply the rule to research-conventions, the MSTID project and the three AI project templates.
- **Sections/Files Affected**: `.claude/commands/commit.md`, `.claude/commands/template-sync.md`, `CLAUDE.md`, `ai/GETTING_STARTED.md`.
- **Nature of Contribution**: Edit of workflow instructions from NAF's verbatim instruction and his acceptance of four proposed refinements.
- **Human Review Status**: Pending review via PR.
- **Git Hash**: `b388d49`, branch `pr-draft-workflow`, PR HamSCI/hamsci-wg#5.
