# ru-text brifly

Reusable Hermes/OpenClaw skill for Russian text quality: typography, editing, info-style, UX writing, business correspondence, anti-pattern diagnostics and text scoring.

Based on an independent Russian text quality reference by Arseniy Kamyshev. Credits and recommended reading are listed in [`references/sources.md`](references/sources.md).

## What is included

- `SKILL.md` — main skill instructions.
- `references/typography.md` — Russian typography rules.
- `references/info-style.md` — clear writing and stop-words.
- `references/ux-writing.md` — UI and microcopy guidance.
- `references/business-writing.md` — emails and business correspondence.
- `references/editorial-grammar.md` — grammar and capitalization.
- `references/editorial-punctuation.md` — punctuation checks.
- `references/anti-patterns.md` — diagnostics and common text problems.
- `references/scoring.md` — quality scoring rubric.
- `references/sources.md` — attribution and recommended reading.
- `agents/` — example agent configurations.

## Install into Hermes

Clone or copy this repository into your Hermes skills directory:

```bash
mkdir -p ~/.hermes/skills/creative
git clone https://github.com/aigalaersh/ru-text_brifly.git ~/.hermes/skills/creative/ru-text
```

Then restart/reload Hermes if your setup does not auto-discover new skills.

## Usage

Trigger examples:

- «вычитай текст»
- «проверь русский»
- «поправь письмо»
- «причеши текст»
- `ru-text`

The skill also contains an always-on typography layer for Russian output.

## Notes

This repository is a portable packaging of the `ru-text` skill. It does not claim endorsement from the authors and publishers listed in `references/sources.md`.
