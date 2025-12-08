# Repository Guidelines

## Project Structure & Module Organization
- `Plan/` holds the four master playbooks (execution plan, daily action guide, funnel optimization guide, KPI dashboard); keep updates modular so other files can cross-reference them.
- `Jira-Tasks/` mirrors the ECM Jira board with day-by-day `.md` tickets (ECM-51 through ECM-59) and a README describing scope and usage.
- `CLAUDE.md` defines canonical campaign context, terminology, and editing expectations—consult it before modifying tactical docs.
- `AGENTS.md` (this file) explains repo conventions; place any new agent-specific notes here for discoverability.

## Build, Test, and Development Commands
- `npx markdownlint-cli2 "**/*.md"` – quick lint of all Markdown files; add `--fix` only after reviewing suggested changes.
- `mdformat Plan/*.md Jira-Tasks/*.md` – optional formatter to normalize spacing and tables (install via `pipx install mdformat` if not already available).
- `rg "□" Plan -n` – sanity check that checkbox glyphs remain intact after edits.
- There is no compile step; use your editor’s Markdown preview to validate tables, checklists, and ASCII timelines.

## Coding Style & Naming Conventions
- Preserve time-block headings in `HH:MM AM/PM` format and keep decision matrices in table form per `CLAUDE.md`.
- Use checkbox syntax (`□` or `- [ ]`) for actionable steps; never mix bullets and checkboxes in the same block.
- New files should follow all-caps snake names (e.g., `WEEK2_GIFT_CARD_PLAN.md`) to match existing artifacts.
- Keep numeric targets explicit (`ROAS 3.0+`, `$45K revenue`); avoid vague statements such as “increase spend.”

## Testing Guidelines
- Treat proofreading as a test: confirm each schedule has metrics, decision criteria, and notes columns before merging.
- Run `npx markdownlint-cli2` and ensure there are no warnings for heading hierarchy or trailing whitespace.
- Confirm cross-file references (e.g., links from Jira tasks to `/Plan`) resolve by opening them in your editor preview.
- When updating formulas, recalc sample rows using spreadsheet mode or a quick scratchpad to ensure KPI math matches `CLAUDE.md`.

## Commit & Pull Request Guidelines
- Prefix commits with the related Jira key (`ECM-53: tighten launch checklist`) or `PLAN:` for cross-cutting docs.
- Commit bodies should summarize the scenario, the change, and any metrics assumptions.
- Pull requests must include: purpose, impacted files, validation notes (lint/proofread), and links to supporting Plan sections or Jira tasks.
- Add screenshots or short clips when you alter visual tables to show alignment/formatting results.

## Agent Workflow Tips
- Start every session by skimming `CLAUDE.md` for constraints, then load the relevant Plan file so you stay in sync with campaign cadence.
- Document any new decision logic or KPI thresholds directly beside the existing tables; duplication elsewhere leads to drift.
- When in doubt, default to the $45K revenue / $10.5K spend targets and the ROAS-based decision tree outlined in the execution plan.
