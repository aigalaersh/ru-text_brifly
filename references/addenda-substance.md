# Addenda: пустота под формой

Ложная антитеза, обязательная триада, выхолощенный механизм, фантомная атрибуция, адресат-поисковик.

Часть свода `addenda.md`. Индекс, Neuroslop index и два правила, управляющие всеми остальными, — там же; читать их до применения любой записи ниже.

## AD-5. Subject-predicate semantic mismatch (семантическое несоответствие субъекта и предиката)

**Problem:** using a predicate whose semantics imply volition, consciousness, resistance, or goal-directed intent, applied to a subject that has none of these. A narrow subset of the broader phenomenon of lexical-semantic compatibility (лексическая сочетаемость / семантическая валентность — Текстология.ру; studme.org).

**Scope restriction (important):** this rule targets only cases where the mismatch creates a **false implication of will, consciousness, resistance, or intent**. It does **not** condemn technical or mathematical personification that has become normative terminology.

**Sources:**
- Лексическая сочетаемость и семантическая валентность: Текстология.ру; studme.org/43201; sci.house/russkiy-yazyik
- Antropomorphism as a recognized cognitive/linguistic phenomenon: Большая Российская Энциклопедия, article «Антропоморфизм»

**Rules:**

AD-5.1. Do not use verbs implying conscious will, resistance, or goal-seeking for subjects that lack them (abstract entities, software without an agent, inanimate processes in non-technical prose).

AD-5.2. **Exception — normative technical terminology.** In mathematical, algorithmic, ML, and general technical writing, the following are legitimate and do not trigger this rule:

  - сходимость алгоритма, последовательность сходится
  - алгоритм стремится к оптимуму / к пределу (mathematical «limit» sense)
  - модель обучается, сеть обучается
  - программа / система принимает решение
  - память компьютера, ответ системы, запрос пользователя

  Rule of thumb: if a domain textbook uses the construction, it is terminology, not anthropomorphism.

AD-5.3. Apply the diagnostic: would a reader infer conscious will or resistance from the predicate? If yes and the subject lacks these properties, rewrite. If the predicate is a technical term or a well-established metaphor (already catalogued in domain usage), leave it.

**Examples:**

| Wrong | Correct | Why |
|---|---|---|
| Модель заставили генерировать числа. | Модели дали задачу генерировать числа. | «заставить» presupposes will to resist |
| Программа не хочет сохранять файл. | Программа не может сохранить файл / отказывается сохранять файл. | «хотеть» implies conscious desire |
| Модель осознала ошибку и исправилась. | Модель выдала ошибку и на следующей итерации — корректный результат. | «осознание» implies reflective consciousness |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| Алгоритм стремится к оптимуму. | Standard optimization terminology (mathematical limit sense). |
| Градиентный спуск сходится к локальному минимуму. | Standard calculus/optimization term. |
| Машина решает задачу за 3 секунды. | Established technical usage — in technical writing such anthropomorphic terms rest on an objective similarity rather than literal animacy (cf. БРЭ, «Антропоморфизм»). |
| Сеть обучается на 10 000 примеров. | Standard ML terminology. |

**Severity:** Low. Secondary signal in the **Ч — Clarity** dimension (supporting **Г — Grammar**), with explicit technical-context exception. Cannot trigger non-compensatory caps alone.

**Acknowledged:** proposed by @V8-Software in issue #9 (2026-04-16) with the example «Алгоритм стремится → Алгоритм становится». That example is preserved here as a *counter-example* illustrating the exception boundary, per deep-research review of mathematical and ML usage norms.


---

---

## AD-6. Manufactured antithesis (ложная антитеза)

**Problem:** a symmetric contrastive-negation pair — «не X, а Y», «это не X, это Y», «X — это не Y. Это Z», «не про X, а про Y», «не потому что X, а потому что Y», «не там, где X, а там, где Y» — where the negated pole X was never voiced in the preceding text and is not a reader expectation the context made explicit. The pair invents a rejected pole only to throw the «true» pole Y into relief, manufacturing rhetorical tension and arguing against an opponent who never spoke. It is one of the strongest machine-generation tells in Russian prose: in measured corpora it appears far more densely in generated text than in live human writing, where the natural device is the opposite: asymmetric self-correction («вернее…», «то есть…», «не то чтобы X, но Y») that refines what was just said. AD-6 targets the manufactured symmetric replacement; the asymmetric refinement is always allowed.

**Sources:**
- Antithesis as a rhetorical figure and the cost of its hollow imitation: editorial practice, informed by Розенталь «Практическая стилистика» on противопоставление
- Distinct from AD-4: AD-4 is a one-sided rebuttal of an unvoiced claim; AD-6 is a two-pole symmetric fork
- Independently formulated from corpus analysis of AI-generated Russian prose

**Trigger constructions:**

- «не X, а Y» / «X, а не Y» — X has no antecedent within the preceding 1–2 paragraphs
- «это не …, это …» / «X — это не Y. Это Z» — two equiweight definitions of one subject, often split by a period
- «не про X, а про Y» / «дело не в X, а в Y» / «вопрос не в X, а в Y» / «суть не в X, а в Y» — the topic swapped through a phantom rejected topic
- «не просто X, а Y» — the hype escalation; flag on the AD-6.1 test, especially when Y is itself inflated («целый», «настоящий», «полноценный»). Hype in Y is a signal, not a standalone trigger
- «не потому что X, а потому что Y» — a cause X that no one supposed
- «не там, где X, а там, где Y» — a locative pseudo-antithesis with no premise
- «не паранойя и не „всё видят“» — a pre-emptive string negating labels nobody put forward
- a cluster of two or more such pairs within ~150 words — density is the strongest signal

**Rules:**

AD-6.1. Flag only when all three conditions hold (any one failing → leave): (1) **no antecedent** — X was not voiced in the preceding 1–2 paragraphs and is not an explicit reader expectation; (2) **symmetry** — X and Y form an equiweight binary of comparable rank and parallel grammar, not a narrowing; (3) **zero increment** — drop the «не X» clause and no fact is lost, Y stands whole.

AD-6.2. Rewrite a flagged pair as a direct positive statement: keep Y, drop the phantom X. «X — это не Y, а Z» → «X — это Z». Do not trade one machine construction for another — removing «не X, а Y» must not introduce «но на самом деле Y» (that is AD-4). Carry the assertion with a fact, a number, an image, or rhythm.

AD-6.3. If the contrast is genuinely needed, earn it: let X be voiced first as a real thesis, a citation, or a reader expectation the context made explicit (the AD-4.3 mechanism). With an antecedent in place, «а Y» is a legitimate antithesis.

AD-6.4. Asymmetric self-correction is never flagged: «вернее…», «то есть…», «по сути…», «не то чтобы X, но Y». Here X is physically present in the preceding clause and the second clause narrows or qualifies the first (refinement, not replacement).

AD-6.5 (quota). Headings: **0** — antithesis in a heading is the loudest tell and reads as clickbait. Sub-headings and leads: rare, and only with a real antecedent in the body (default 0). Body: **0–2** legitimate pairs per article (antecedent present, or concrete data on both poles). Manufactured pairs are always 0 regardless of the limit; self-corrections and antecedent-backed antitheses are not counted toward it.

AD-6.6. Single-count with neighbours. A phantom contrast can also read as AD-4 (one-sided rebuttal) or AD-2 (parcellation when split on periods). Count one violation per fragment: AD-6 takes precedence for a symmetric two-pole fork; a one-sided «но на самом деле…» with no named counter-pole stays AD-4. Do not double-charge Structure.

AD-6.7 (scope of strengthening). The trigger set now includes «не просто X, а Y» and «вопрос/суть не в X, а в Y». Two look-alikes are NOT auto-flagged: «не столько X, сколько Y» (a degree-narrowing, cf. AD-6.4) and «важно не X, а Y» without an antecedent (often a real reader priority). A cluster of manufactured pairs bites harder in **С — Structure** (see `scoring.md`); the carve-outs hold — asymmetric self-correction (AD-6.4) and the 0–2 legitimate antecedent-backed body pairs (AD-6.5) are never penalised, and the construction is never banned outright.

AD-6.8 (the quota is not a finding). AD-6.5 sets how many pairs a text may carry; it is not a line to report in place of them. Report each manufactured pair with its own fragment and let the count raise the weight in **С — Structure**. In a measured run a checker reported «два и более на ~150 слов» and dropped one of the pairs it was counting.

**Examples:**

| Wrong | Correct |
|---|---|
| Это не баг, а фича. | Так и задумано. |
| Это не про скорость, а про надёжность. | Это про надёжность. |
| ИИ — это не инструмент. Это образ мышления. | ИИ меняет то, как я думаю о задаче. |
| Дело не в модели, а в промпте. | Всё решает промпт. |
| Не медленно, а быстро. | Отвечает за 200 мс. |
| Это не просто инструмент, а целая экосистема. | Это экосистема: редактор, отладчик, пакетный менеджер. |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| Хочу и буду. Вернее, буду, когда хочу. | Asymmetric self-correction: X is present, the second clause narrows it. |
| Это не неуверенность — это точность мышления вслух. | The negated pole is a real reader misreading the context invites (antecedent satisfied). |
| Выросло не на 2%, а на 40%. | Both poles carry data; deletion loses information. |
| Не мытьём, так катаньем. | Fixed idiom. |
| Не оферта, а приглашение делать оферты. | Legal formula where the binary is operative semantics. |
| Не столько баг, сколько недокументированное поведение. | Degree-narrowing («не столько… сколько»): X is present and partly true, the clause refines rather than replaces (cf. AD-6.4). |
| Он сделал это не просто так, а с умыслом. | «не просто так» is a fixed idiom («for a reason»), not the «не просто X, а Y» hype escalation. |

**Severity:** Medium — the manufactured antithesis is the single strongest machine-generation tell in this addenda set, and density compounds fast. Primary signal in the **С — Structure** dimension (supporting **Ч — Clarity**), reflected in the С rubric anchors. A cluster of manufactured pairs materially lowers the С score; a single antecedent-backed pair does not. Still cannot, by itself, trigger a non-compensatory cap — that stays reserved for the hard dimensions and the global < 3.0 floor.

**Acknowledged:** identified from corpus analysis of AI-generated Russian prose (2026-06); the contrastive-negation antithesis runs at high density in machine drafts and near-zero in human reference corpora.


---

---

## AD-11. Mandatory tricolon (обязательная триада)

**Problem:** enumerations that arrive in threes because three is the shape, not because the subject has three parts — «инновационный, трансформирующий, прорывной». The rule of three is a real device with a long rhetorical history; the tell is its automatic application. The giveaways are that the third member rewords the first two, that the members are of unequal rank, and above all that the pattern repeats: a text where every list is three items long is being written by a form, not about a subject.

**Sources:**
- Expressive syntax and the cost of a figure applied mechanically: editorial practice, informed by Розенталь «Справочник по правописанию и стилистике»
- `info-style.md` §B — the unproven-claim adjectives that most often fill the three slots
- AD-7 already names the self-praise tricolon about one's own product; AD-11 is the general case and the two are kept apart by AD-11.5
- Independently formulated from the 2026 review of AI-generated Russian prose

**Trigger constructions:**

- three adjectives in a row, none of them measurable — «инновационный, трансформирующий, прорывной»
- three noun phrases where the third rewords the first two
- every heading in a section followed by exactly three bullets
- «во-первых… во-вторых… в-третьих» where the third point restates the first
- the strongest signal: two or more forced triples in one text

**Rules:**

AD-11.1. Flag a triple when all three hold: (1) the subject does not have exactly three parts — a fourth could be added, or one dropped, with nothing lost; (2) the members are not distinct — one repeats or contains another; (3) deleting a member loses no fact. Density is part of the test, not a separate remark: a cluster of two or more such triples in one text is the primary signal, and an isolated triple is flagged only when every member is an unproven claim from `info-style.md` §B.

AD-11.2. Rewrite by keeping what carries information: two members with distinct content, or one member with a number behind it.

AD-11.3 (density raises severity; it never replaces the findings). Report **each** forced triple with its own fragment and let the cluster raise the weight in **С — Structure**. See «Two rules that govern all the others» for why.

AD-11.4 (carve-out — the subject has three). An exhaustive enumeration — «рожковые, капсульные и автоматические» — three real steps, three measurements, three named parties: not flagged. This is AD-11.1's first test decided the other way: no fourth member could exist, so the three belong to the subject rather than to the form.

AD-11.5 (single-count with AD-7). A triple that praises the author's own product or delivery — «быстро, надёжно, красиво» — is AD-7's self-praise tricolon and is charged there, in **Ч — Clarity**. AD-11 takes the forced triple that is not self-praise, in **С — Structure**. Never both for one fragment.

AD-11.6 (single-count with info-style §B — the SAME fragment only). Where the members of the triple are §B unproven adjectives, count that fragment once: §B when the defect is the missing evidence, AD-11 when it is the forced count. Never both **for that fragment**. An unproven adjective elsewhere in the sentence — «хороший процесс должен быть прозрачным, предсказуемым и управляемым», where «хороший» is the subject and not a member — is a separate defect and is reported separately. Single-count means one charge per fragment, never one charge per sentence.

AD-11.7 (carve-out — oratorical and literary register). The tricolon is a legitimate figure in speeches, manifestos and literary prose, where rhythm is part of the work (cf. AD-2.3, which likewise spares the literary register).

**Examples:**

| Wrong | Correct |
|---|---|
| Инструмент инновационный, трансформирующий и прорывной. | Инструмент собирает отчёт за 4 с вместо 3 мин. |
| Процесс должен быть прозрачным, предсказуемым и управляемым. | Процесс должен быть предсказуемым: срок известен на старте. |
| Он меняет подход к планированию, к оценке и к контролю. | Он меняет оценку сроков. |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| Кофемашины бывают рожковые, капсульные и автоматические. | Exhaustive enumeration: no fourth type exists (AD-11.4). |
| Задержку определяют три вещи: расстояние, загрузка канала и версия протокола. | Three distinct mechanisms, each named (AD-11.4, cf. AD-12.3). |
| Сначала открываем конфиг, затем меняем порт, затем перезапускаем сервис. | Three real steps of a procedure. |
| Мы измеряли в Москве, Франкфурте и Сингапуре. | Three named places, each carrying its own datum. |

**Severity:** Low. Secondary signal in the **С — Structure** dimension (supporting **Ч — Clarity**). A cluster lowers Structure; an isolated triple does not. Cannot trigger non-compensatory caps alone.

**Acknowledged:** identified in the 2026 neuroslop review, from a reader-complaint channel where the forced three was named repeatedly and independently of any single model family.


---

---

## AD-12. Hollowed mechanism (выхолощенность)

**Problem:** a claim that something matters, with the operative term replaced by a placeholder — «зависит от различных факторов», «есть целый ряд причин», «имеет свои особенности», «определённая специфика». The sentence has the shape of an explanation and none of its content: the reader cannot act on it, check it, or disagree with it, because nothing has been said. It is the most economical way for a paragraph to pass for informative. Not to be confused with AD-3: AD-3 says the same thing twice, AD-12 says nothing once.

**Sources:**
- `info-style.md` §E — a claim without a number or a source is an opinion; §B lists «определённый» among the stop-words with the instruction to name the specific thing
- `info-style.md` §D — the worked contrast between «различные проблемы» and a problem named
- `editorial-grammar.md` §E.2 — «следует учитывать следующие факторы» is catalogued there as a tautology (the cognate pair «следует… следующие»): the neighbouring defect is the wording, the defect here is the emptiness
- Independently formulated from the 2026 review of AI-generated Russian prose

**Trigger constructions:**

- «различные факторы» / «ряд факторов» / «целый ряд причин» / «по ряду причин»
- «свои особенности» / «своя специфика» / «определённая специфика» / «известные нюансы»
- «многие аспекты» / «те или иные» / «в той или иной степени» / «разный эффект»
- «зависит от многого» / «всё индивидуально» / «зависит от ситуации» as a whole answer
- «играет важную роль» / «имеет большое значение» where neither the role nor the significance is named (cf. AD-13)

**Rules:**

AD-12.1. Flag a clause when all three hold: (1) it asserts influence, dependence, importance or difficulty; (2) the term carrying the mechanism is a placeholder rather than a name — «факторы», «аспекты», «особенности», «специфика», «моменты», «нюансы» are the common ones, and so is any bare quantifier or degree word standing in for the mechanism: «многое», «те или иные», «в той или иной степени», «разный», «большое значение». The list is open; the test is whether the word tells the reader WHICH; (3) nothing in the piece names what the placeholder stands for — not this sentence, not its neighbours, and not a section, table or source the sentence points to (AD-12.3).

AD-12.2. Rewrite by naming: replace the placeholder with the two or three actual items. If they cannot be named, the sentence was not knowledge, and deleting it loses nothing.

AD-12.3 (carve-out — the placeholder is cashed out, here or elsewhere). «Задержку определяют три вещи: расстояние до дата-центра, загрузка канала и версия протокола» — the placeholder is a colon away from its content. It counts just as much when the cash-out is deferred by an explicit pointer: «объясняется рядом факторов, разобранных в разделе 4», a reference to a table, an appendix, or a named source. That is the normal convention of technical, normative and academic writing, and the window is the whole document — the same reach AD-13.3 gives an attribution named once and referred to later. The defect is the placeholder that stays empty, not the one answered on another page.

AD-12.4 (carve-out — honest uncertainty). A stated limit of knowledge that says what is unknown and why — «мы не знаем, откуда разброс: замеры шли на разном железе» — is information. The target is a pretence of an answer, never the admission that there is none.

AD-12.5 (single-count with info-style §B). «Определённый» is already a §B stop-word. Charge the fragment once: §B when the defect is the empty determiner, AD-12 when it is the unnamed mechanism. Never both.

AD-12.6 (single-count with AD-13). A clause can carry both defects in two different fragments — «исследования показывают, что влияют различные факторы» is AD-13 on the attribution and AD-12 on the mechanism, which is two fragments and two charges. One fragment is never charged to both.

**Examples:**

| Wrong | Correct |
|---|---|
| Результат зависит от различных факторов. | Результат зависит от версии протокола и от загрузки канала. |
| У каждого проекта своя специфика. | В этом проекте два подрядчика и общий репозиторий. |
| Многие аспекты процесса изучены недостаточно. | Мы не измеряли, как влияет размер команды. |
| Мотивация имеет большое значение. | Команды с недельным циклом обратной связи закрывали задачи на 20% быстрее. |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| Задержку определяют три вещи: расстояние, загрузка канала и версия протокола. | The placeholder is cashed out in the same sentence (AD-12.3). |
| Мы не знаем, откуда разброс: замеры шли на разном железе. | Honest uncertainty, with the reason named (AD-12.4). |
| Специфика ГОСТ 8.417 в том, что единицы пишутся без точки. | «Специфика» followed by the specific thing. |

**Severity:** Medium — a text made of these sentences is indistinguishable in shape from an informative one, which is exactly what makes it expensive. Primary signal in the **Ц — Reader precision** dimension (supporting **Ч — Clarity**), reflected in the Ц rubric anchors. Two or more hollowed clauses land Ц in the 5–6 band or lower. Cannot trigger a non-compensatory cap alone.

**Acknowledged:** identified in the 2026 neuroslop review from a reader-complaint channel; checked against the corpus before proposing, where the pattern was found absent — the nearest neighbours are a tautology entry about the wording and a worked example about a different point.


---

---

## AD-13. Phantom attribution (неопределённая атрибуция)

**Problem:** the gesture of citing, without a source — «исследования показывают», «эксперты отмечают», «учёные доказали», «по мнению аналитиков». The sentence borrows the authority of a body of work that is never identified, so the reader cannot go and look. This is worse than an unsupported claim, not better: a bare claim invites the question «откуда это?», while a dressed one discourages it. Distinct from the unproven-claim adjectives of `info-style.md` §B — there no source is offered at all, here a source is imitated.

**Sources:**
- `info-style.md` §E — a number or claim without a source is an opinion, not a fact
- Adjacent to AD-10: both perform an authority instead of holding one
- Independently formulated from the 2026 review of AI-generated Russian prose

**Trigger constructions:**

- «исследования показывают» / «согласно исследованиям» / «учёные доказали»
- «эксперты отмечают» / «специалисты рекомендуют» / «аналитики прогнозируют»
- «принято считать» / «общеизвестно, что» / «как показывает практика» / «статистика говорит»
- «играет ключевую роль» — a rank assigned with nobody ranking and no criterion given. Where the defect is the missing mechanism rather than the missing source, AD-12 is the home; charge the fragment once
- the strongest signal: an attribution that no sentence in the piece ever redeems

**Rules:**

AD-13.1. Flag an attribution when the source is not identifiable anywhere in the text: no author, organisation, publication, date or link, here or elsewhere in the piece.

AD-13.2. Rewrite by naming the source, or by dropping the attribution and owning the claim. «Исследования показывают, что удалёнка снижает продуктивность» → «По данным опроса N (2025, 1 200 респондентов), …» or «На наших четырёх проектах продуктивность упала».

AD-13.3 (carve-out — a real source). Named, dated and checkable — «По данным Росстата за 2025 год» — is not flagged, and neither is a later reference to a source the piece named once.

AD-13.4 (carve-out — consensus with a citation). Where the existence of a consensus is itself the point and a citation follows, «принято считать» is a legitimate framing move rather than a phantom.

AD-13.5 (carve-out — marked personal experience). «По моему опыту», «у нас на проекте», «в трёх наших внедрениях» attribute to the author, who is identifiable and answerable. That is a source.

AD-13.6 (single-count with info-style §B). An unproven adjective and a phantom attribution in one fragment are one charge: §B when the defect is the unevidenced claim, AD-13 when it is the imitated citation. Never both.

**Examples:**

| Wrong | Correct |
|---|---|
| Исследования показывают, что удалёнка снижает продуктивность. | По данным опроса Института X (2025, 1 200 респондентов), продуктивность упала на 8%. |
| Эксперты отмечают: рынок вырастет. | ЦБ в июльском прогнозе ждёт роста на 3%. |
| Учёные доказали, что кофе полезен. | (delete, or cite the study) |
| Мотивация играет ключевую роль. | Без обратной связи в первую неделю уходит каждый третий новичок. |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| По данным Росстата за 2025 год, зарплата выросла на 12%. | Named, dated, checkable (AD-13.3). |
| По моему опыту, миграции такого размера занимают неделю. | Attributed to the author, who is answerable (AD-13.5). |
| Принято считать, что индексы ускоряют чтение; замер ниже это опровергает. | Consensus named in order to be tested, and it is (AD-13.4). |

**Severity:** Medium — an imitated citation does more damage than a missing one, because it suppresses the reader's question. Primary signal in the **Ц — Reader precision** dimension (supporting **Ч — Clarity**), reflected in the Ц rubric anchors. Cannot trigger a non-compensatory cap alone.

**Acknowledged:** identified in the 2026 neuroslop review from a reader-complaint channel; checked against the corpus before proposing, where the pattern had no entry of any kind.


---

---

## AD-15. Search-engine addressee (адресат — поисковик, а не читатель)

**Problem:** the implied reader is a crawler. Nothing in the text is ungrammatical and no single sentence is wrong; the piece is simply not addressed to a person. The query phrase is repeated verbatim where a language addressed to a reader would use a pronoun; sections are variants of one question rather than steps of an argument; and after reading, the reader still cannot do the thing the piece is about. Two platforms formulate the test the same way, and both formulate it as a question of **addressee** rather than of provenance.

**Sources:**
- Habr's site rules as they stood on 27.07.2026 (the version announced 17.06.2026) name material aimed at search engines rather than living readers among the content it restricts (paraphrased, not quoted)
- Яндекс Вебмастер lists automatically generated *and* useless-to-the-user content among the examples its algorithms may restrict; the conjunction is operative — machine origin alone is not the stated violation (paraphrased, not quoted)
- `info-style.md` §A (полезное действие) and §D (main point first) — the two properties such a text lacks
- `scoring.md` notes that formula tools score an SEO text highly without any real quality; that is the observation, and this rule is the judgement it calls for
- **The sentence-level signature below is this corpus's own formulation.** Neither platform states what the tell looks like inside a sentence; only the criterion of addressee is theirs

**Trigger constructions:**

- the exact query phrase repeated verbatim in the title, in a heading, and again in the body
- headings that are variants of one another rather than steps — «как выбрать X», «какие бывают X», «сколько стоит X»
- the subject named by its full noun phrase where a pronoun or a short form would serve
- a «выводы» section that restates the headings and adds no number
- length without a fact: the piece answers a query and leaves the reader unable to act

**Rules:**

AD-15.1. Charge the document when all three hold: (1) a query phrase is repeated where the language would use a pronoun or a short form; (2) sections are variants of one question rather than steps of an argument; (3) after reading, a reader cannot do the thing the piece is about — no number, no criterion, no named option.

AD-15.2. Rewrite by answering the question once and with specifics: name the options and the criterion by which one is chosen, with prices where they decide it.

AD-15.3 (carve-out — the user's explicit brief). Where the user asks for SEO copy, the style priority stated in `SKILL.md` applies: their request overrides these defaults. State what the trade-off costs and write what was asked.

AD-15.4 (carve-out — functional repetition). Technical writing repeats an identifier because a pronoun would be ambiguous — «поле `updated_at` меняется при каждой записи, поле `created_at` — нет». Reference works, glossaries and legal texts repeat the term by design. The defect is the addressee, not the repetition.

AD-15.5 (carve-out — optimisation that still serves the reader). Keyword research legitimately shapes what a useful text covers. A piece that answers the query with facts is not flagged for having the query in its title.

AD-15.6 (level — the document charge ADDS, it never replaces). A note on what the repetition is and is not: `editorial-grammar.md` §E defines tautology as ADJACENT cognates and pleonasm as words duplicating each other's meaning, so a query phrase repeated across four paragraphs is neither, and the corpus has no separate rule for distant lexical repetition. That repetition is AD-15's own evidence and belongs to AD-15 alone — do not borrow a Г finding the corpus does not carry. Like AD-14, this rule is charged to the document, and the repetitions are the evidence for that one charge rather than one AD-15 finding each. That is the **only** thing it absorbs. Every other defect in the same text is reported exactly as it would be without this rule: the stop-words and unproven claims in **Ч**, any pleonasm or tautology the corpus already catalogues in **Г** (`editorial-grammar.md` §E), the passive constructions, the missing полезное действие, the headings that are not theses. A summary that costs the writer the list of lines to fix is not a summary (see «Two rules that govern all the others»).

**Examples:**

| Wrong | Correct |
|---|---|
| Купить кофемашину в Москве: как выбрать кофемашину для дома | Как выбрать кофемашину для дома |
| Цена кофемашины зависит от типа кофемашины и производителя кофемашины. | Цена зависит от типа и производителя: рожковые — от 12 000 ₽, автоматические — от 40 000 ₽. |
| Раздел «Как выбрать кофемашину для дома: выводы», пересказывающий предыдущие заголовки | Раздел с рекомендацией: какая модель кому подходит и почему |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| Поле `updated_at` меняется при каждой записи, поле `created_at` — нет. | Repetition because a pronoun would be ambiguous (AD-15.4). |
| Заголовок «Как выбрать кофемашину» над текстом с ценами и критериями | The query is answered with facts (AD-15.5). |
| Глоссарий, где термин повторён в каждой статье | Reference format (AD-15.4). |

**Severity:** High — like AD-14, the defect is the piece rather than a phrase in it, and the reader's loss is total: the text is about their question and gives them nothing. Primary signal in the **Ц — Reader precision** dimension (supporting **С — Structure**), reflected in the Ц rubric anchors: a document charged with AD-15 does not reach the upper Ц bands. It does **not** introduce a new non-compensatory cap (see `scoring.md`).

**Acknowledged:** identified in the 2026 neuroslop review from the editorial-policy channel, where two platforms independently formulated the same test of implied addressee.


---

---

## AD-16. Additive pseudo-pair («не только X, но и Y»)

**Problem:** a pair joined by «не только… но и», «как… так и», «и… и», in which the second pole adds nothing — it rewords the first, or is contained in it, or both are empty. The construction promises an increment and delivers a rhythm. It is the neighbour of AD-6 and not the same rule: there an opposition with no antecedent, here an addition with no content.

**Sources:**
- `editorial-grammar.md` — the corpus's only «не только… но и» entry is a predicate-agreement rule, a different subject entirely; the two do not collide
- Informed by a 2025 linguo-pragmatic study of AI-assisted Russian social-media posts (cf. Оломская, Юрова; CyberLeninka), which counts the construction among the clichés it treats as markers of generated text. **The density threshold is this corpus's own caution, not the study's finding:** the study measured 38 posts of one political-SMM channel, a genre that reaches for the construction anyway, so the frequency it reports cannot carry a per-sentence rule and the threshold keeps an isolated pair out of the flag
- Distinct from AD-6 (see AD-16.5)
- Independently formulated from the 2026 review of AI-generated Russian prose

**Trigger constructions:**

- «не только X, но и Y» where Y rewords X or is contained in it
- «как X, так и Y» with the same defect
- «и X, и Y» with synonymous poles
- a cluster of two or more such pairs in a short text — density is the signal

**Rules:**

AD-16.1. Flag a pair when all three hold: (1) **no increment** — Y states nothing X did not; (2) **not a contrast** — this is addition, so it is not AD-6 and must not be charged there; (3) **deletable** — drop «не только» and one pole, and no fact is lost. Density belongs to the test: two or more such pairs in one text is the signal, and an isolated pair is not flagged.

AD-16.2. Rewrite as the single claim that survives, and give it something to stand on: «не только удобный, но и комфортный» → name what the interface does, in one step, with a number if there is one.

AD-16.3 (carve-out — a real pair). «Не только в Москве, но и в Новосибирске: 12 мс и 47 мс» — AD-16.1's increment test decided the other way: each pole carries its own number, and deleting either loses it.

AD-16.4 (carve-out — scope). «Не только для физлиц, но и для ИП» defines who is covered. Scope-widening is operative content, frequently legal, and is never flagged.

AD-16.5 (single-count with AD-6). A fragment is charged once. AD-6 takes a symmetric opposition whose negated pole has no antecedent; AD-16 takes an addition whose second pole has no content. If a construction reads as both, it is almost always AD-6 — check for a rejected pole before charging here.

AD-16.6 (single-count with info-style §B — the SAME fragment only). Where both poles are §B unproven adjectives, count that fragment once: §B for the missing evidence, AD-16 for the empty pair. An unproven adjective outside the pair stays its own finding; single-count is per fragment, never per sentence.

AD-16.7 (density raises severity; it never replaces the findings). Report **each** pair with its own fragment and let the count raise the weight. See «Two rules that govern all the others».

AD-16.8 (the pair and the synonymy are two defects, not one). «Не только удобный, но и комфортный» carries both: the poles are synonyms, which is a pleonasm and belongs where pleonasms have always belonged — `editorial-grammar.md` §E, in **Г — Grammar** — and the frame adds nothing, which is AD-16, in **С — Structure**. They are separable, and that is the test: «Сервис удобный и комфортный» is the pleonasm with no pair; «не только быстрее, но и дешевле» with two real numbers behind it is neither. Where both hold, report both. In a measured run, folding the pleonasm into AD-16 scored the same text **higher than before the rule against it existed** — Grammar recovered its points because the finding had moved to a Low signal in another dimension. A new rule against a text must never make that text score better.

**Examples:**

| Wrong | Correct |
|---|---|
| Сервис не только удобный, но и комфортный. | Сервис открывает отчёт в два клика вместо семи. |
| Платформа помогает не только экономить время, но и тратить его меньше. | Платформа сокращает сборку отчёта с 3 мин до 4 с. |
| Мы предлагаем как качественные решения, так и решения высокого уровня. | Мы делаем интеграции с 1С и с SAP. |
| Обновление затрагивает не только интерфейс, но и внешний вид. | Обновление меняет интерфейс. |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| Мы измеряли не только в Москве, но и в Новосибирске: 12 мс и 47 мс. | Both poles carry data (AD-16.3). |
| Скидка действует не только для физлиц, но и для ИП. | Scope-widening: operative content (AD-16.4). |
| Не только студенты, но и преподаватель присутствовал. | The corpus's agreement example: a different rule about a different thing. |

**Severity:** Low. Secondary signal in the **С — Structure** dimension (supporting **Ч — Clarity**). Density is the signal; an isolated pair is not flagged at all. Cannot trigger non-compensatory caps alone.

**Acknowledged:** identified in the 2026 neuroslop review from the linguistic channel; checked against the corpus before proposing, where the construction appears exactly once and as a rule about predicate agreement.
