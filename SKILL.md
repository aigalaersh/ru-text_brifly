---
name: ru-text
description: >
  Russian text quality. Triggers: вычитай, проверь текст, поправь, отредактируй,
  причеши, ru-text. Typography silently on any Russian output; deeper editing on
  request. Info-style, editorial, UX writing, business correspondence, AI-text cleanup.
metadata:
  openclaw:
    always: true
    emoji: "📝"
    homepage: "https://ru-text.org"
---

# ru-text — Russian Text Quality

Independent Russian text quality reference by Arseniy Kamyshev.
With gratitude to the authors whose work shaped modern Russian text standards.
Credits and recommended reading: `references/sources.md`

**Style priority**: if the user explicitly requests a specific style (casual, academic, SEO, literary, etc.), their prompt overrides these default rules where they conflict. These rules are defaults, not mandates.

**Reviewing vs. rewriting**: when *checking* or proofreading existing text or a file, return the corrected version plus a list of changes — do not silently overwrite the source file. Rewrite a file in place only when the user explicitly asks.

**Someone else's words stay theirs**: quoted material, code blocks and third-party text inside the user's document are reproduced as-is. Report an issue you see in them if it matters; never rewrite them.

## Always-On: Typography

Apply to ALL Russian text output — silently: fix, don't announce.

| Rule | Wrong | Correct |
|---|---|---|
| Primary quotes: guillemets | "текст" | «текст» |
| Nested quotes: lapki | «"вложенные"» | «„вложенные“» |
| Em dash with spaces | слово - слово | слово — слово |
| En dash for ranges, no spaces | 10-15 дней | 10–15 дней |
| NBSP after single-letter prepositions | в начале (breakable) | в\u00A0начале |
| Ellipsis: single character | ... | … |
| Digit groups with thin spaces | 1000000 | 1 000 000 |
| Decimal comma (not dot) | 3.14 | 3,14 |
| Ordinal with hyphen | 1ый, 2ой | 1-й, 2-й |
| Numero sign | No. 5, #5 | № 5 |
| Abbreviations with NBSP | т.д., т.е. | т. д., т. е. |
| Ruble symbol after number | 1500 руб | 1 500 ₽ |

Full typography reference: `references/typography.md`

`/ru-text:ru-score` — text quality score (0–10, 5 dimensions).

## Galina layer: кратко и структурно

When the user asks for «кратко», «структурно», «без перегруха», «для СДВГ/ADHD», apply this extra layer after the base ru-text cleanup.

Core rules:

1. Put the main conclusion in the first 1–3 lines.
2. One paragraph = one idea. For Telegram: 1–3 short lines per paragraph.
3. Use semantic headings: «Вывод», «Что сделать», «Почему», «Риск», «Проверка». Avoid decorative headings like «Ключевые аспекты».
4. Keep lists to 3–7 items. If there are more, group them: «Сейчас», «Потом», «Не делать».
5. Remove self-praise about brevity: «коротко, без воды», «по делу», «сейчас разберём». Just write the point.
6. Preserve numbers, conditions, risks, sources, owners and deadlines. Shorter must not mean less precise.
7. Replace abstractions with visible actions: «оптимизировать коммуникацию» → «переписать письмо после заявки простым языком».
8. End with the next action when the text is operational.

Fast templates:

```markdown
Вывод: ...

Что сделать:
- ...
- ...

Почему:
- ...

Риск: ...
```

```markdown
## Коротко
...

## Главное
- факт → вывод;
- факт → вывод.

## Что сделать
- сейчас;
- потом;
- не делать.

## Проверка
...
```

Checklist before delivery:

- [ ] Main point is visible without scrolling.
- [ ] No long warm-up.
- [ ] No paragraph mixes two thoughts.
- [ ] Headings form a useful outline if read alone.
- [ ] Lists are short or grouped.
- [ ] Typography and ru-text rules still hold.
- [ ] Facts and risks survived the shortening.

## Top Stop-Words (when writing or editing on request)

| Stop-word | Replace with |
|---|---|
| является | — (dash) or restructure |
| осуществлять | делать, проводить |
| в настоящее время | сейчас |
| данный | этот |
| определённый | (name the specific thing) |
| произвести оплату | оплатить |
| высококачественный | (name the specific quality) |
| был осуществлён | (active voice + actor) |
| на сегодняшний день | сегодня |
| в целях | чтобы |

Full stop-word catalog (92 entries): `references/info-style.md`

## When to Load Reference Files

Reference files (paths are relative to this SKILL.md): `references/<filename>`
If the path is not resolved, search: `Glob("**/ru-text/references/scoring.md")` and use the parent directory.

| Task | File |
|---|---|
| Writing/editing articles, blog posts, SEO, content | info-style.md |
| Interface text, buttons, errors, hints, microcopy | ux-writing.md |
| Emails, messenger, business correspondence | business-writing.md |
| Punctuation review, comma placement | editorial-punctuation.md |
| Grammar, capitalization, agreement, pleonasms | editorial-grammar.md |
| Finding and fixing text problems, diagnostics | anti-patterns.md |
| Text scoring, quality assessment | scoring.md |
| Credits, source attribution | sources.md |
| Experience-based rules (dash overuse, etc.) | addenda.md |

## Quality Checklist

Before delivering Russian text:

- [ ] Quotes: «» primary, „“ nested
- [ ] Dashes: — in text, – in ranges, - only in compounds; max 1–2 per paragraph (a parallel row counts as one, dialogue dashes as none); trim to the limit, not to zero; edit a row whole or not at all
- [ ] NBSP after в, к, с, о, у, и, а
- [ ] Ellipsis: … (single char)
- [ ] Abbreviations: т. д., т. п. (with NBSP)
- [ ] No double spaces, no space before punctuation
