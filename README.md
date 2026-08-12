# ru-text brifly

Переносимый скилл качества русского текста: типографика, редактура, информационный стиль,
UX-writing, деловая переписка, диагностика нейросетевого стиля и оценка текста по рубрике.

Основан на независимом справочнике по качеству русского текста Арсения Камышева. Благодарности
и список источников — в [`references/sources.md`](references/sources.md).

## Что внутри

| Файл | О чём |
|---|---|
| `SKILL.md` | основные инструкции: always-on-типографика, краткий режим, маршрутизация |
| `commands/ru-check.md` | команда `/ru-text:ru-check` — вычитка со списком правок |
| `commands/ru-score.md` | команда `/ru-text:ru-score` — оценка 0–10 по пяти измерениям |
| `references/typography.md` | правила русской типографики (R1–R96) |
| `references/info-style.md` | информационный стиль, каталог стоп-слов |
| `references/ux-writing.md` | интерфейсные тексты и микрокопирайт |
| `references/business-writing.md` | письма и деловая переписка |
| `references/editorial-grammar.md` | грамматика, прописные, согласование (разделы C–K) |
| `references/editorial-punctuation.md` | пунктуация (разделы A–B) |
| `references/anti-patterns.md` | каталог ошибок по степени тяжести |
| `references/scoring.md` | рубрика оценки |
| `references/addenda.md` | индекс свода AD: Neuroslop index и маршрутизация |
| `references/addenda-rhythm.md` | AD-1, AD-2, AD-17, AD-18 — ритм, пунктуация, знаки |
| `references/addenda-register.md` | AD-3, AD-4, AD-7…AD-10, AD-14 — регистр ассистента |
| `references/addenda-substance.md` | AD-5, AD-6, AD-11…AD-13, AD-15, AD-16 — пустота под формой |
| `references/sources.md` | атрибуция и что читать дальше |

## Установка

Hermes:

```bash
mkdir -p ~/.hermes/skills/creative
git clone https://github.com/aigalaersh/ru-text_brifly.git ~/.hermes/skills/creative/ru-text
```

Claude Code:

```bash
git clone https://github.com/aigalaersh/ru-text_brifly.git ~/.claude/skills/ru-text
```

Имя каталога должно совпадать с полем `name` в `SKILL.md` — то есть `ru-text`, а не
`ru-text_brifly`. Если харнесс не подхватывает скиллы сам, перезапустите его.

## Как вызывается

- «вычитай текст», «проверь русский», «поправь письмо», «причеши текст», `ru-text`;
- «кратко», «структурно», «без перегруза» — краткий режим;
- «убери воду», «не пиши как нейросеть» — разбор по Neuroslop index;
- `/ru-text:ru-check`, `/ru-text:ru-score` — команды.

**Про «always-on».** Флаг `metadata.openclaw.always` понимает openclaw. В Claude Code и
большинстве других харнессов скилл подключается по описанию, поэтому типографика применяется
не ко всему выводу подряд, а начиная с момента, когда скилл загружен в разговор. Если нужна
типографика по умолчанию — вызовите скилл в начале сессии или закрепите его настройками
харнесса.

## Границы

Типографика правит прозу и не трогает машиночитаемые строки: код, пути, URL, версии, флаги
команд, регулярные выражения, числа для CSV, JSON, YAML и SQL. Полный список — раздел
«Do not touch (scope limits)» в `SKILL.md`. Чужие слова — цитаты и сторонние вставки —
воспроизводятся как есть.

## Лицензия

MIT, см. [`LICENSE`](LICENSE). Лицензия распространяется на формулировки правил в этом
репозитории; книги, статьи и инструменты из `sources.md` принадлежат их авторам и здесь не
воспроизводятся. Репозиторий не заявляет одобрения со стороны перечисленных там авторов
и издателей.

История изменений — [`CHANGELOG.md`](CHANGELOG.md).
