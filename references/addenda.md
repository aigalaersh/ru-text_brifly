# Addenda — rules added from usage experience

The rules below were added later, from real editorial practice, and were not part of the
plugin's initial rule set. Like the rest of the plugin, they are independently formulated; the
16 sources in `sources.md` informed the work, but no rule is taken or copied from them. They are
supported by academic references. Kept separate for traceability: initial rule set vs. experiential
additions.

## Как читать этот свод

Свод разбит на четыре файла. Этот — индекс: он даёт Neuroslop index, два правила,
управляющие всеми остальными, и таблицу маршрутизации. Сами записи AD лежат в трёх
тематических файлах и читаются по одной: грузить нужный файл, а не весь свод.

| Файл | О чём | Записи |
|---|---|---|
| `addenda-rhythm.md` | ритм, пунктуация, знаки | AD-1, AD-2, AD-17, AD-18 |
| `addenda-register.md` | регистр ассистента | AD-3, AD-4, AD-7, AD-8, AD-9, AD-10, AD-14 |
| `addenda-substance.md` | пустота под формой | AD-5, AD-6, AD-11, AD-12, AD-13, AD-15, AD-16 |

Ссылки вида «AD-7.4 (`addenda.md`)» в других файлах ведут сюда: запись ищется по таблице ниже.

## Table of Contents

| Запись | Название | Файл |
|---|---|---|
| AD-1 | Excessive em dashes (избыточные тире) | `addenda-rhythm.md` |
| AD-2 | Excessive parcellation (избыточная парцелляция) | `addenda-rhythm.md` |
| AD-3 | Patronizing explanation (разжёвывание очевидного) | `addenda-register.md` |
| AD-4 | Unprovoked rebuttal (возражение без предпосылок) | `addenda-register.md` |
| AD-5 | Subject-predicate semantic mismatch (семантическое несоответствие субъекта и предиката) | `addenda-substance.md` |
| AD-6 | Manufactured antithesis (ложная антитеза) | `addenda-substance.md` |
| AD-7 | Preemptive virtue qualifier (непрошенная оговорка «без воды») | `addenda-register.md` |
| AD-8 | Assistant-register meta-commentary (сервисные реплики ассистента) | `addenda-register.md` |
| AD-9 | Hollow opener (пустой зачин) | `addenda-register.md` |
| AD-10 | Declared sincerity (объявленная искренность) | `addenda-register.md` |
| AD-11 | Mandatory tricolon (обязательная триада) | `addenda-substance.md` |
| AD-12 | Hollowed mechanism (выхолощенность) | `addenda-substance.md` |
| AD-13 | Phantom attribution (неопределённая атрибуция) | `addenda-substance.md` |
| AD-14 | Chat transcript as the artifact (диалог с нейросетью вместо текста) | `addenda-register.md` |
| AD-15 | Search-engine addressee (адресат — поисковик, а не читатель) | `addenda-substance.md` |
| AD-16 | Additive pseudo-pair («не только X, но и Y») | `addenda-substance.md` |
| AD-17 | Comma welded to a dash (запятая, сомкнутая с тире) | `addenda-rhythm.md` |
| AD-18 | Uppercase band vs. deliberate emphasis (капслок: полоса против выделения) | `addenda-rhythm.md` |

## Neuroslop index

A compact catalogue of the recurring tells of AI-generated Russian prose, each routed to the rule
that is its canonical home. These tells skew by training era and instruction-tuning style rather
than by any single vendor; a breakdown by specific model family is intentionally omitted as
unverifiable and fast-dating.

| Tell | Canonical home |
|---|---|
| Manufactured antithesis — «не X, а Y» / «не просто X, а Y» with no antecedent | AD-6 (`addenda-substance.md`) |
| Declared sincerity — «честный разбор», «давайте будем честны», «рассказываю как есть» | AD-10 (`addenda-register.md`) |
| Mandatory tricolon — «инновационный, трансформирующий, прорывной» | AD-11 (`addenda-substance.md`) |
| Hollowed mechanism — «зависит от различных факторов», «свои особенности» | AD-12 (`addenda-substance.md`) |
| Phantom attribution — «исследования показывают», «эксперты отмечают» | AD-13 (`addenda-substance.md`) |
| Chat transcript as the artifact — «Я: … / Модель: …» as the document's skeleton | AD-14 (`addenda-register.md`) |
| Search-engine addressee — the query phrase repeated where a pronoun would serve | AD-15 (`addenda-substance.md`) |
| Additive pseudo-pair — «не только X, но и Y» where Y adds nothing | AD-16 (`addenda-substance.md`) |
| Preemptive virtue qualifier — «без воды», «чётко, по делу», «коротко и ясно» | AD-7 (`addenda-register.md`) |
| Assistant-register meta-commentary — «Отличный вопрос!», «Надеюсь, это помогло» | AD-8 (`addenda-register.md`) |
| Hollow opener — «давайте разберёмся», «погрузимся», «важно понимать, что» | AD-9 (`addenda-register.md`) |
| Excessive em dashes — staccato dash rhythm | AD-1 (`addenda-rhythm.md`) |
| Comma welded to a dash — «…, — …» inside one sentence | AD-17 (`addenda-rhythm.md`) |
| Throat-clearing stop-words — «стоит отметить, что», «нельзя не отметить» | `info-style.md` §B |
| Empty universal preamble — «в современном мире», «не секрет, что» | `info-style.md` §B |
| Unproven-claim adjectives — «качественный», «надёжный», «эффективный» | `info-style.md` §B |
| Generic conclusion — «таким образом, подводя итог» | `anti-patterns.md` |
| Artificial liveliness — exclamation stacks and emoji as a substitute for detail | `info-style.md` §F |

## Two rules that govern all the others

**Density raises severity; it never replaces the findings.** Several rules here treat a
cluster as their main signal — AD-1, AD-2, AD-6, AD-9, AD-11, AD-16. Once a rule has
decided that it fires, report every instance, individually, with its own quoted fragment,
and let the count govern how far the score moves. One line saying «два и более на текст» in
place of the four fragments is a loss of coverage wearing the clothes of a summary: the
person fixing the text is left without the list of lines to fix.

This says nothing about **whether** a rule fires. Two of the six — AD-11 and AD-16 — put
density into the flag condition itself, so an isolated triple or an isolated pair is not a
finding at all; that is their own text and it stands. The rule here governs what happens
after a rule has decided to fire, never before.

Nor is the score card a limit on what the check reports: `scoring.md` asks for one to
three issues per dimension in the scored output; that is the size of a table cell, not the
size of the check. `/ru-text:ru-check` lists what it found; `/ru-text:ru-score` quotes the
most telling of them per dimension. Neither number licenses dropping a finding.

**A document-level charge adds; it never replaces.** AD-14 and AD-15 are charged to the
piece as a whole. Each absorbs only its own evidence — the repetitions that demonstrate it
— and absorbs nothing else. Every ordinary finding in that text stands: stop-words,
unproven claims, passive voice, punctuation, typography. Both statements exist because a
measured run did the opposite: it replaced ten ordinary findings with three document-level
ones, and the text came out looking better for it.

---
