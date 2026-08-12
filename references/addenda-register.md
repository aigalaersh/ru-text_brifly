# Addenda: регистр ассистента

Сервисные реплики, пустые зачины, объявленная искренность, разжёвывание, диалог вместо текста.

Часть свода `addenda.md`. Индекс, Neuroslop index и два правила, управляющие всеми остальными, — там же; читать их до применения любой записи ниже.

## AD-3. Patronizing explanation (разжёвывание очевидного)

**Problem:** explaining what the context has already conveyed treats the reader as unable to make simple inferences. Over-explanation lowers pace, lowers trust, and adds words without information.

> **Not to be confused with** *примитивизация* as used in `info-style.md` section A, point 2: «Сокращение — забота о читателе, **не примитивизация**.» There «примитивизация» means oversimplification at the cost of meaning (e.g., removing necessary qualifiers). This rule concerns the opposite failure: redundant explanation of what the sentence has already conveyed. Both rules defend reader intelligence — from different directions.

**Sources:**
- Editorial practice around «respect the reader's intelligence»: cf. N. Gal, Ilyakhov
- Over-explaining in writing: liminalpages.com, writing.codidact.com/posts/75048
- `info-style.md` section A, point 2 — companion principle (against the opposite failure)

**Rules:**

AD-3.1. If a sentence already conveys a fact, do not immediately re-state it in a simpler metaphor or reformulation.

AD-3.2. Numeric comparisons that are self-evident to the reader do not need verbal paraphrase.

AD-3.3. Qualifiers like «то есть», «другими словами», «проще говоря» are warning signs — verify that the following clause actually adds information, not just rewords the preceding one.

**Examples:**

| Wrong | Correct |
|---|---|
| Конверсия выросла с 2% до 8%, то есть стала в четыре раза больше. | Конверсия выросла с 2% до 8%. |
| Мы сократили расходы на 30% — это почти треть бюджета. | Мы сократили расходы на 30%. |
| Пользователи тратят 12 минут, другими словами, больше десяти. | Пользователи тратят 12 минут. |

**Severity:** Low. Secondary signal in the **Ч — Clarity** dimension. Cannot trigger non-compensatory caps alone.

**Acknowledged:** proposed by @V8-Software in issue #9 (2026-04-16) as «Примитивизация»; renamed to avoid terminological collision with `info-style.md` A.2.

---

---

## AD-4. Unprovoked rebuttal (возражение без предпосылок)

**Problem:** constructions like «а это уже…», «но на самом деле…», «однако в реальности…» presuppose a prior claim that the writer is now refuting. When no such claim exists in the preceding text, the rebuttal invents an imaginary opponent and creates a non-existent conflict (cf. straw man / non-sequitur).

**Sources:**
- Straw-man fallacy and non-sequitur: Grammarly; Scribbr; Excelsior Online Writing Lab
- The rhetorical idea that a speaker argues against an opponent who may be real or imagined: HSE «Риторика» (nnov.hse.ru)

**Trigger constructions:**

- «а это уже [нечто важное/серьёзное]»
- «но на самом деле…», «на самом-то деле…»
- «однако в реальности…», «однако на практике…»
- «но при этом нужно понимать, что…»
- «только вот…»

**Rules:**

AD-4.1. Before any adversative construction, verify that the preceding text (within the same section or 1–2 paragraphs back) contains a claim that is actually being rebutted.

AD-4.2. If no antecedent exists, rewrite as a direct positive statement — remove the pseudo-rebuttal scaffolding.

AD-4.3. Legitimate use: rebutting a cited source, an earlier paragraph of the same text, or a reader expectation that the context makes explicit.

**Examples:**

| Wrong | Correct |
|---|---|
| …а это уже реальный сценарий, в котором модели постоянно обучают друг друга. | …данных, которыми модели постоянно обучают друг друга. |
| Но на самом деле алгоритм обрабатывает 10 000 запросов в секунду. | Алгоритм обрабатывает 10 000 запросов в секунду. |
| Однако в реальности пользователь открывает приложение раз в день. | Пользователь открывает приложение раз в день. |

**Severity:** Low. Secondary signal in the **С — Structure** dimension (supporting **Ч — Clarity**). Cannot trigger non-compensatory caps alone.

**Acknowledged:** proposed by @V8-Software in issue #9 (2026-04-16).

---

---

## AD-7. Preemptive virtue qualifier (непрошенная оговорка «без воды»)

**Problem:** a trailing manner-flourish that asserts the author's virtue by denying a fault the reader never raised — «без воды», «без виляния», «без лишних слов», «начистоту», «честно говоря», «прямо скажем», «не побоюсь этого слова», «и без всякой магии». The statement reassures the reader against a vice nobody suspected, so the qualifier carries no information and only performs sincerity. It is a cousin of AD-4: where AD-4 rebuts an unvoiced external claim, AD-7 denies an unvoiced fault of the author's own delivery. The same flourish also appears in positive polarity — «чётко, по делу», «коротко и ясно», «простыми словами», «разложу по полочкам» — naming a delivery virtue the text should simply demonstrate; it is flagged identically. Virtue is shown by the writing, never announced.

**Sources:**
- Telling vs. showing, and self-praise as an empty signal: editorial practice, informed by Нора Галь «Слово живое и мёртвое» on needless self-qualification
- Adjacent to AD-4 (unprovoked rebuttal) and AD-3 (patronizing explanation)
- Independently formulated from corpus analysis of AI-generated Russian prose

**Trigger constructions:**

- «без воды» / «без виляния» / «без лишних слов» / «без обиняков» — a manner-flourish denying a vice of delivery
- «честно говоря» / «начистоту» / «прямо скажем» / «не побоюсь этого слова» — announced sincerity
- «скажу честно» / «если честно» / «честно» / «по-честному» / «не буду врать» / «откровенно говоря» / «положа руку на сердце» — the same announced sincerity in the forms a model reaches for most. Where the sincerity is predicated of the whole piece rather than of one statement — «честный разбор», «давайте будем честны» — the home is AD-10; charge the fragment once (AD-10.6)
- «и без всякой магии» / «без всяких фокусов» / «без нервов» appended to a claim about one's own product or method
- «чётко, по делу» / «коротко и ясно» / «простыми словами» / «разложу по полочкам» / «на пальцах» — a positive-form flourish praising the author's own delivery (the polarity twin of «без воды»)
- a self-praise tricolon about one's own product or method — «быстро, качественно, надёжно» — where each adjective is itself an unproven claim (cf. `info-style.md` §B) and the rule-of-three stacking is the added tell
- a virtue adverb stacked on a self-statement where deleting it loses no fact

**Rules:**

AD-7.1. Flag a preemptive virtue qualifier — whatever its surface form, including a «без [vice]» phrase, announced sincerity in any syntactic form (parenthetical «честно говоря», finite verb «скажу честно», bare adverb «честно»), a positive-form delivery flourish, a self-praise tricolon, and a virtue adverb stacked on a self-statement — when it (1) characterises the author's own product, delivery or method, (2) answers an objection the text never raised, whether by denying the vice or by asserting its opposite, and (3) carries no information — deleting it loses no fact. The carve-outs of AD-7.3, AD-7.4, AD-7.5 and AD-7.7 apply to every branch of this test, the positive-polarity branch included: an informative «без», a genuine epistemic qualifier, a speaker inside the text, a qualifier previewing concrete content that immediately follows, and an established genre or rubric label are not flagged.

AD-7.2. Rewrite by deleting the qualifier and letting the statement stand; the virtue is demonstrated by the writing. «Соберу мысль, без виляния» → «Соберу мысль».

AD-7.3. Allow informative «без»: «кофе без сахара», «работает без интернета», «ноль vi.*-моков, без заглушек», «без регистрации» — here «без» names a real removed ingredient, dependency, or feature, not a manner.

AD-7.4. Allow a genuine epistemic qualifier that carries information: «строго говоря, это аппроксимация», «по сути» when it narrows the claim (cf. AD-6.4). These calibrate meaning; they do not advertise sincerity.

AD-7.5 (register — whose voice it is). The carve-out holds when the construction belongs to a **speaker inside the text**: a line of dialogue, a quotation, an interviewee, a character. «— Скажу честно, я не знаю, — ответил инженер» is speech and is not flagged. It does **not** hold when the author says it about their own text, in any register — an author addressing the reader in a conversational tone is still the author, and «скажу честно» in a lead is the self-promotional flourish AD-7.1 describes, not spoken connective tissue. This is a deliberate narrowing: the earlier wording exempted the conversational register as such, and the assistant register — a monologue written to sound like speech — fell straight through it, which is how a construction listed among the triggers went unflagged for a year. AD-10.4 is the canonical statement of this boundary; it governs both rules, and is stated there in full because a rule read on its own must decide on its own.

AD-7.6. Single-count with neighbours. A «без [vice]» flourish can also be caught by AD-2 (parcellation / filler rhythm in Structure) — the «без воды» tail in «Расскажу последовательно, доступно, без воды» is one fragment, not two faults. Count one violation per fragment: charge it to AD-7 (**Ч — Clarity**) when the defect is the empty self-virtue, to AD-2 (**С — Structure**) when the defect is the staccato or filler rhythm. Never double-charge the same fragment across Ч and С.

AD-7.7. Positive-form delivery self-praise is flagged under AD-7.1: it is the positive-polarity branch of clause (2), and two carve-outs apply to it specifically. «Объясню чётко, по делу» → «Объясню» (then actually do). Do NOT flag a qualifier that previews concrete content that immediately follows: «Объясню коротко: значение лежит в стеке» carries information about what comes next and stays. An established genre or rubric label — a column or book title «… на пальцах», «… простыми словами» — is a recognised popular-science convention, not a delivery flourish, and is not flagged.

AD-7.8 (single-count with info-style §B). The unproven-claim tricolon «быстро, качественно, надёжно» is also three §B unproven adjectives (`info-style.md` §B, «качественный»/«надёжный»/«эффективный» family). Count it once in **Ч — Clarity**: charge AD-7 when the defect is the self-virtue rule-of-three, or info-style §B when the defect is the missing evidence per the domain brief — never both for the same fragment.

**Examples:**

| Wrong | Correct |
|---|---|
| Соберу мысль, без виляния. | Соберу мысль. |
| Отвечу честно, без воды: дедлайн сорван. | Дедлайн сорван. |
| Скажу прямо, без обиняков: тест не проходит. | Тест не проходит. |
| Это работает, и без всякой магии. | Это работает. |
| Max 20× закрывает запрос начисто, без нервов. | Max 20× закрывает запрос. |
| Объясню чётко, по делу, без воды. | Объясню. |
| Расскажу простыми словами, разложу по полочкам. | Расскажу. |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| Кофе без сахара. | «без» names a real removed ingredient. |
| Ноль vi.*-моков — без заглушек. | «без» names a real removed thing. |
| Сервис работает без интернета. | «без» names a real capability. |
| Строго говоря, это аппроксимация. | Epistemic qualifier carrying real information. |
| Объясню коротко: значение лежит в стеке. | «коротко» previews concrete content that immediately follows (AD-7.7). |
| Работает быстро: ответ за 200 мс. | A speed claim backed by a number, not a self-virtue flourish. |

**Severity:** Low. Secondary signal in the **Ч — Clarity** dimension (supporting **С — Structure**). Cannot trigger non-compensatory caps alone.

**Acknowledged:** identified from corpus analysis of AI-generated Russian prose (2026-06); the «без [vice]» self-virtue flourish recurs in machine drafts and reads as announced rather than demonstrated quality.


---

---

## AD-8. Assistant-register meta-commentary (сервисные реплики ассистента)

**Problem:** a chatbot-persona flourish that addresses the reader as a live interlocutor or narrates the helping transaction instead of carrying the subject — a sycophantic acknowledgement of the question («Отличный вопрос!», «Прекрасная идея», «Вы абсолютно правы»), or an assistant sign-off offering further help («Надеюсь, это помогло», «Готов помочь», «Обращайтесь, если что»). It breaks the fourth wall of written prose: it talks about the helping exchange rather than delivering content. A cousin of AD-7 — both perform a stance instead of demonstrating it — but distinct in that AD-7 praises the text's quality while AD-8 performs the assistant's service persona.

**Sources:**
- Telling vs. showing, and respect for the reader's time: editorial practice, informed by Нора Галь «Слово живое и мёртвое»
- Adjacent to AD-7 (preemptive virtue) and to business-writing email-closing norms
- Independently formulated from corpus analysis of AI-generated Russian prose

**Trigger constructions:**

- «Отличный вопрос!» / «Прекрасный вопрос» / «Хороший вопрос» / «Прекрасная идея» / «Вы абсолютно правы» — a sycophantic acknowledgement of the reader as interlocutor
- «Надеюсь, это помогло» / «Надеюсь, было полезно» / «Готов помочь» / «Обращайтесь, если что» / «Если будут вопросы — спрашивайте» — an assistant sign-off offering further help
- «Сейчас всё объясню» / «Давайте я расскажу» narrating the helping process where no real internal cross-reference is meant

**Rules:**

AD-8.1. Flag a flourish that (1) addresses the reader as a conversational interlocutor or narrates the helping transaction, and (2) carries zero subject content — deleting it loses no fact and the surrounding text stands whole.

AD-8.2. Rewrite by deleting the flourish: open with the answer, end on the last substantive point. «Отличный вопрос! Давайте посмотрим…» → start with the answer.

AD-8.3. Cross-reference, not double-charge. A genuine call to action with a real channel in correspondence — «пишите на support@…», «звоните в будни» — is business-writing territory, and an over-bloated email closing is already covered (cf. `business-writing.md:158`, `anti-patterns.md:90`). AD-8 targets the persona leak into article or documentation prose, not a real email CTA; charge a given fragment once.

AD-8.4 (register carve-out). Not flagged in genuine live dialogue, chat-support exchanges, or interview and quoted registers, where the speaker is responding to a real interlocutor: a support reply «Спасибо за обращение! Подскажите номер заказа», or «„Хороший вопрос“, — ответил инженер», is natural discourse (cf. AD-2.3, AD-7.5). A standalone «Готов помочь» in a real contact or footer block is a genuine offer, not meta-commentary. A sincere authorial wish in a book preface, foreword, or acknowledgements («надеюсь, книга окажется полезной») is a conventional register, not a chat-persona leak. The target is the assistant persona injected into monologue or educational prose, not a one-way FAQ that answers anticipated questions.

AD-8.5. Single-count with neighbours. A sign-off that also reads as filler rhythm can be caught by AD-2; charge the empty-persona defect to AD-8 (**Ч — Clarity**), the staccato or filler defect to AD-2 (**С — Structure**). Never double-charge the same fragment.

**Examples:**

| Wrong | Correct |
|---|---|
| Отличный вопрос! Давайте разберёмся. | (delete; open with the answer) |
| Вы абсолютно правы, и вот почему. | Вот почему. |
| Надеюсь, это было полезно. Обращайтесь! | (delete; end on the last substantive point) |
| Готов помочь с любыми вопросами по теме. | (delete) |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| Спасибо за обращение! Подскажите номер заказа. | Real support dialogue with a live user. |
| Если остались вопросы по договору — пишите на support@example.com. | Genuine CTA with a real channel (cf. business-writing.md:158). |
| «Хороший вопрос», — ответил инженер. | Quoted dialogue / interview register. |
| Вы правы: в расчёте действительно ошибка. | A genuine concession in real correspondence, carrying a fact. |

**Severity:** Low. Secondary signal in the **Ч — Clarity** dimension (supporting **С — Structure** at lead and closer position). Cannot trigger non-compensatory caps alone.

**Acknowledged:** identified from corpus analysis of AI-generated Russian prose (2026-06); the assistant-persona flourish leaks the chat register into monologue text and reads as service performance rather than content.


---

---

## AD-9. Hollow opener (пустой зачин)

**Problem:** an opening or transitional flourish that announces explanation instead of delivering it — «давайте разберёмся», «давайте погрузимся», «копнём глубже», «разложим по полочкам», «важно понимать, что», and «итак» used as filler. The lead carries no fact; it only clears the throat before the real first sentence. It works against the inverted pyramid (`info-style.md` §D: the main point goes first, and the first sentence is the paragraph's thesis). The strongest signal is density — a cluster of such openers, one per paragraph, padding a text that never quite begins.

**Sources:**
- Main point first, first sentence as thesis: `info-style.md` §D (structure)
- The throat-clearing openers «стоит отметить, что» / «не секрет, что» are already catalogued as stop-words in `info-style.md` §B (see AD-9.3)
- Independently formulated from corpus analysis of AI-generated Russian prose

**Trigger constructions:**

- «давайте разберёмся» / «давайте погрузимся» / «копнём глубже» / «разложим по полочкам» — a narrated descent into the topic with no content
- «важно понимать, что» / «здесь важно понять» / «нужно понимать» — a hedged preamble before a claim
- «итак,» / «как известно,» used as a paragraph opener that introduces nothing new
- a lead whose only content is the promise to explain
- the strongest signal: a cluster of two or more such openers within a short section (~200 words)

**Rules:**

AD-9.1. Flag an opener or transition that (1) announces explanation rather than delivering it, and (2) carries zero increment — deleting it loses no fact and the next sentence stands as the real lead. A cluster of two or more hollow openers in a paragraph or short section is the primary signal; an isolated instance is weak.

AD-9.2. Rewrite by deleting the flourish and promoting the first substantive sentence to the lead (`info-style.md` §D).

AD-9.3 (single-count with info-style §B). The throat-clearing openers «стоит отметить, что», «следует подчеркнуть», «нельзя не отметить», «не секрет, что», «в современном мире» are already stop-words in `info-style.md` §B — apply them there and count once. AD-9 adds the dive-in family («давайте разберёмся», «погрузимся», «важно понимать») not listed in §B, plus the cluster signal. Never charge one fragment to both §B and AD-9.

AD-9.4 (carve-out — genuine connective). «Итак» as a real summative connective that closes a reasoning chain, or a resumptive connective that picks up a narrative thread (cf. `editorial-punctuation.md:119`), is not flagged; only the empty opener «Итак,» that introduces nothing.

AD-9.5 (carve-out — real tutorial). «Давайте разберём» / «давайте посмотрим» in a genuine step-by-step walkthrough, where the next sentence actually begins with concrete steps, is not flagged. The target is the decorative promise with no follow-through.

AD-9.6 (carve-out — informative «важно»). «Важно понимать разницу между TCP и UDP — от неё зависит выбор протокола» carries a real consequence and is not flagged (analogous to AD-7.4). Flag only the empty hedge.

AD-9.7 (carve-out — dialogue register). «Давайте разберёмся» / «давайте посмотрим» in genuine live dialogue or a quoted or interview register, where a real interlocutor proposes to look into something together, is natural speech, not a hollow opener (cf. AD-7.5, AD-8.4).

**Examples:**

| Wrong | Correct |
|---|---|
| Давайте разберёмся, как это работает. | Алгоритм делает три вещи: … |
| В этой статье мы погрузимся в мир машинного обучения. | Машинное обучение… (open with the subject) |
| Важно понимать, что скорость зависит от железа. | Скорость зависит от железа. |
| Итак, что же мы имеем? | (delete; state what we have) |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| Итак, из трёх замеров следует: задержка не выше 200 мс. | Genuine summative connective closing a chain (cf. editorial-punctuation.md:119). |
| Давайте разберём по шагам. Шаг 1: откройте файл. | Real tutorial; the next sentence delivers concrete steps. |
| Важно понимать разницу между TCP и UDP — от неё зависит выбор протокола. | The «важно» clause carries a real consequence (cf. AD-7.4). |

**Severity:** Low. Secondary signal in the **С — Structure** dimension (supporting **Ч — Clarity**). A cluster lowers Structure; an isolated opener does not. Cannot trigger non-compensatory caps alone.

**Acknowledged:** identified from corpus analysis of AI-generated Russian prose (2026-06); the hollow opener announces explanation instead of leading with the point and clusters densely in machine drafts.


---

---

## AD-10. Declared sincerity (объявленная искренность)

**Problem:** the text asserts its own honesty as a property of itself — «честный разбор», «давайте
будем честны», «рассказываю как есть», «без прикрас», «вся правда о…». Sincerity is what a reader
infers from what a text does with an inconvenient fact; announced, it is a claim with no evidence,
and it takes the place of the evidence that would have earned it. AD-7 catches the same reflex
attached to one statement («скажу честно: дедлайн сорван»); AD-10 catches it when honesty is
predicated of the piece or of the block that follows. The label form is the louder of the two and is
graded accordingly, and giving it its own name is what lets the carve-out be stated once instead of
twice.

**Sources:**
- Telling vs. showing, and self-praise as an empty signal: editorial practice, informed by Нора Галь «Слово живое и мёртвое»
- Platform moderation practice treats stylistic resemblance as sufficient grounds on its own, without proof of generation — Habr's site rules as they stood on 27.07.2026, the version announced in the platform's own post of 17.06.2026 (paraphrased, not quoted); this is external evidence that a style-level rule has a real object
- Adjacent to AD-7 (delivery-virtue qualifier) and AD-13 (phantom attribution): all three perform a stance instead of demonstrating it
- Independently formulated from the 2026 review of AI-generated Russian prose

**Trigger constructions:**

- «честный разбор» / «честный обзор» / «честно о…» / «вся правда о…» / «без прикрас» — the piece labelled honest, most often in a title
- «давайте будем честны» / «будем откровенны» / «скажем прямо» opening a paragraph or a section
- «рассказываю как есть» / «пишу как думаю» / «без купюр» / «начистоту»
- a title or lead whose only claim is the author's own sincerity
- the strongest signal: the label in a heading, where the reader has been given nothing yet against which to weigh it

**Rules:**

AD-10.1. Flag a construction when all three hold: (1) it predicates honesty, frankness or candour of the text, of the author's account, or of the block that follows; (2) the author is speaking about their own text; (3) it carries no fact — deleting it loses nothing.

AD-10.2. Rewrite by deleting the label and letting the inconvenient fact do the work it was standing in for. «Честный разбор: почему сроки срываются» → «Почему сроки срываются» — and then name the reason.

AD-10.3. Honesty is demonstrated specifically: an admitted mistake, a number that costs the author something, a stated limit of what is known. Where the demonstration is present the label is redundant; where it is absent the label is false.

AD-10.4 (carve-out — the speaker inside the text). Not flagged when the construction belongs to a speaker inside the text: a line of dialogue, a quotation, an interviewee, a character. «— Скажу честно, я не знаю, — ответил инженер» is speech, not a label. This is the canonical statement of the boundary the narrowed AD-7.5 applies: the carve-out protects a voice inside the text, never the author speaking about their own text.

AD-10.5 (carve-out — informative «честный»). «Честная цена» meaning a price with no hidden fees, «честный вес», «честный тест» meaning one whose method is published — here «честный» names a checkable property of the object, not a virtue of the prose (compare AD-7.3).

AD-10.6 (single-count with AD-7). One fragment, one charge. AD-10 takes it when honesty is predicated of the text or frames what follows; AD-7 takes it when the qualifier modifies a single statement in the flow. Never both.

**Examples:**

| Wrong | Correct |
|---|---|
| Честный разбор: почему проекты срываются | Почему проекты срываются |
| Давайте будем честны — планировать умеет не каждая команда. | Из двенадцати команд в срок уложились три. |
| Рассказываю как есть, без прикрас. | (delete; then tell it) |
| Вся правда о подписках. | Что входит в подписку и что нет. |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| — Скажу честно, я не знаю, — ответил инженер. | Speech of a person inside the text (AD-10.4). |
| Честная цена: 4 900 ₽, доставка входит. | «Честный» names a checkable property of the object (AD-10.5). |
| Мы ошиблись в расчёте на 30% и потеряли квартал. | Honesty demonstrated rather than announced (AD-10.3). |
| Строго говоря, это аппроксимация. | Epistemic qualifier carrying information (cf. AD-7.4). |

**Severity:** Medium — the label form is the most conspicuous member of the declared-sincerity family and the one a reader notices first. Primary signal in the **Ч — Clarity** dimension (supporting **Ц — Reader precision**), reflected in the Ч rubric anchors. A label in a heading, or two instances in one text, materially lowers Ч; a single one in the body does not. Still cannot, by itself, trigger a non-compensatory cap.

**Acknowledged:** identified in the 2026 neuroslop review, from a reader-complaint channel and from a probe the author supplied — «скажу честно». That exact form was in no trigger list; its close relative «честно говоря» was, among AD-7's, and the register carve-out then exempted it. So the family was named and the coverage was not, which is the same failure the probe exposed.


---

---

## AD-14. Chat transcript as the artifact (диалог с нейросетью вместо текста)

**Problem:** the published piece is the log of a conversation with a model. Its skeleton is a sequence of turns rather than an argument: questions become headings, answers become sections, and the piece ends when the conversation did. The reader is handed the raw material and asked to do the author's work on it. This is one of the set's two rules charged to the **document** rather than to a fragment — the other is AD-15 — and no local edit removes either, because the defect is the shape.

**Sources:**
- Platform editorial policy names this artifact directly: Habr's site rules as they stood on 27.07.2026 (the version announced 17.06.2026) list, among material that should not be posted, pieces that are the author's dialogues with neural networks and pieces consisting only of model answers; a separate section of the same rules restricts unfinished drafts and streams of consciousness (paraphrased, not quoted)
- Distinct from AD-8, which flags an assistant reply leaking into monologue prose: that is a sentence, this is a skeleton (see AD-14.5)
- `info-style.md` §D — the inverted pyramid a transcript cannot have, because a conversation is ordered by turns
- Independently formulated from the 2026 review of AI-generated Russian prose

**Trigger constructions:**

- alternating speaker labels — «Я:» / «Модель:», «Пользователь:» / «Ответ:», «Промпт:» / «Результат:»
- the piece's headings are the questions that were asked
- prompt echo: each answer restates the question before answering it
- the closing is the end of the exchange — «Спасибо, теперь понятно» — rather than a conclusion
- no sentence in the piece is a claim of the author's own

**Rules:**

AD-14.1. Charge the document when both hold: (1) its structure is a sequence of exchanges rather than an exposition; (2) the author contributes no claim of their own — no thesis, no synthesis, no assessment of what the model said.

AD-14.2. Rewrite by writing the piece: state what you learned, in the order a reader needs it, and keep from the transcript only what a reader must see in order to check you.

AD-14.3 (level — the document charge ADDS, it never replaces). AD-14 is a property of the whole document: attach it once, not to an individual line, and a single quoted exchange inside an ordinary article is not this rule at all. The charge adds one finding and replaces none: every defect inside the transcript is reported as it would be otherwise (see «Two rules that govern all the others»).

AD-14.4 (carve-out — the transcript as evidence). A log published as evidence for the author's own finding, with the finding stated and the log subordinate to it, is not flagged: a prompt-engineering write-up, a documented experiment, a bug report, a reproduction. The test is one deletion: remove the log — does a claim of the author's remain? If yes, the log was evidence.

AD-14.5 (relationship to AD-8 — not a double charge). AD-8 flags individual assistant replies inside a text; AD-14 flags the text's shape. Repair every AD-8 flourish and an AD-14 document is still a transcript; repair the shape and the flourishes were never the problem. The two defects survive each other's repair, so both are charged — this is not one fragment counted twice.

AD-14.6 (carve-out — human dialogue). An interview, a Q&A with a human respondent, a play, a chat-support excerpt, a quoted exchange: dialogue between people is a genre, not a tell (cf. AD-8.4).

AD-14.7 (carve-out — the transcript was what was asked for). Where the user's brief is a transcript — documentation of a session, a teaching example showing prompts and outputs — the style priority stated in `SKILL.md` applies and these defaults do not override the request.

**Examples:**

| Wrong | Correct |
|---|---|
| **Я:** Объясни кеширование. **Модель:** Отличный вопрос! … | ETag сравнивает версию ресурса; при совпадении сервер отвечает 304. (then the author's own account) |
| Заголовок раздела: «А что такое ETag?» | Заголовок раздела: «ETag: когда сервер отвечает 304» |
| Закрытие: «Спасибо, теперь понятно.» | Закрытие: вывод, ради которого текст написан. |

**Counter-examples (do NOT flag):**

| Acceptable | Reason |
|---|---|
| Ниже — расшифровка: я задал модели один вопрос трижды и свёл ответы в таблицу. Разброс — вывод статьи. | The log is evidence for the author's own finding (AD-14.4). |
| «Хороший вопрос», — ответил инженер. | Quoted human dialogue (AD-14.6, cf. AD-8.4). |
| Интервью с разработчиком, вопрос — ответ. | An interview is a genre. |

**Severity:** High — the highest in this addenda set, and it means something specific: the defect is not a fragment to repair but the form of the piece, so no sequence of local edits removes it. Primary signal in the **С — Structure** dimension (supporting **Ц — Reader precision**), reflected in the С rubric anchors: a document charged with AD-14 does not reach the upper Structure bands. It does **not** introduce a new non-compensatory cap — those stay reserved for the hard dimensions and the global floor (see `scoring.md`). Severity here says how far the dimension moves, not that a new cap exists.

**Acknowledged:** identified in the 2026 neuroslop review from the editorial-policy channel, where a Russian platform names the artifact in its own rules rather than in commentary.


---
