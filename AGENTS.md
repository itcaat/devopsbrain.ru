# Repository Agent Instructions

## Writing and Editing Articles

Apply these rules when drafting, reviewing, restructuring, or editing articles in this repository. The Kafka series is the reference for the intended approach: approachable Russian prose, technical precision, a continuing practical example, and explanations that build on one another.

### Voice and Language

- Write like an experienced engineer explaining a system to a curious colleague, not like a glossary, a translated manual, or marketing copy.
- Use simple, natural Russian without sacrificing technical meaning. Prefer concrete actions and actors over abstract noun chains and awkward literal translations.
- Keep an authorial voice where it helps: "Давайте разберёмся", "Теперь посмотрим", "Я рекомендую". Do not mechanically add "мы с вами" to every section. Explain the reason and trade-off behind a recommendation.
- Do not invent the author's production experience, incidents, benchmarks, or personal preferences. Hypothetical product examples must not sound like reported real-world cases.
- Avoid vague claims such as "это повышает надёжность" without explaining what failure is handled, how, and what remains outside the guarantee.
- Keep established technical terms in English consistently across the series: Producer, Consumer, Broker, Topic, Partition, Consumer Group, Leader, Followers. Explain a term naturally on first use; do not repeatedly switch between translations and transliterations.
- Use code formatting for exact configuration names, values, fields, APIs, and code. Do not wrap every mention of a technical concept in backticks. Keep identifiers consistent, for example `orderId` rather than alternating with `OrderID` and `OrderId`.

Examples of the intended language:

- Instead of "повторы Producer", write "Producer повторно отправляет сообщение при временной ошибке" or "автоматические повторные отправки".
- Instead of "прочитанное сообщение не обязано исчезать", write "чтение сообщения не удаляет его из журнала; оно остаётся доступным согласно политике хранения".
- Instead of merely saying that more Partition improve performance, first explain the bottleneck and why additional independent logs allow more work to run concurrently.

### Build an Explanation, Not a List of Terms

- Start from a practical question or problem the reader can already understand. Introduce a mechanism as an answer to that question, not just because it is the next term to define.
- A useful progression is: problem, mechanism, concrete example, consequence, limitations. Use it flexibly rather than forcing every section into the same template.
- Before using a concept, check whether the reader has received enough background. Define it briefly when needed, or postpone the detail until the prerequisites are established.
- Connect sections through their meaning. For example: Value explains what happened, Key helps choose a Partition, and Offset identifies the position inside that Partition. Avoid a sequence of isolated dictionary entries.
- Explain why a change is needed before describing its consequences. Before discussing increasing the Partition count, establish the load or parallelism problem that motivates it.
- Use concrete product scenarios, identifiers, timelines, and failure outcomes. Examples should distinguish mechanisms, not make different settings look interchangeable. For example, explain what acknowledgement `acks=1` provides that `acks=0` does not, and what risk remains.
- State the scope of guarantees and important assumptions. Distinguish writing to Kafka from completing a business operation, reading from processing, and retries from idempotency.
- Do not turn a useful simplification into an unconditional claim: avoid promises of linear scaling, absence of all locks, universal zero-copy, or in-memory performance without qualification.
- Describe independent or concurrent actions as such. Do not present background disk flush, replication, and Consumer reads as mandatory consecutive stages.
- Add a small number of links to relevant official documentation at points where deeper detail is genuinely useful. Verify the linked page and claim; do not link every term or interrupt every paragraph.

### Continuity Across a Series

- Read the target article and the relevant preceding and following sections before editing. Check both prerequisites and transitions, not only local wording.
- Keep one recognizable example through the series. In the Kafka series, continue the internet store, its services, order events, Topic names, and identifiers instead of introducing a new store in each part.
- Briefly recall the relevant established fact, then develop it. Do not repeat the full explanation of a mechanism already covered, such as replication and `acks`.
- Make the evolution of an example explicit. When a simple payload becomes a production event contract, explain that metadata is being added to the earlier simplified representation.
- Give each part one central question and a manageable number of new concepts. Split substantially denser articles by learning objective rather than by an arbitrary word count.
- End with a natural bridge to the next question. Prefer general references such as "далее" or "в следующих частях" rather than promises tied to specific future part numbers. Existing navigation links can still name the parts.
- When splitting or reordering articles, update titles, descriptions, series metadata, navigation, announcements, and affected internal links. Preserve published paths where possible; handle redirects deliberately if a path must change.

### Editing Scope and Review

- Preserve the author's useful phrasing and edits. Improve the requested issue without automatically rewriting the whole article or changing its voice.
- If asked to review or discuss, report findings before editing. If asked to fix specific items, limit changes to those items and directly necessary follow-up adjustments.
- Prefer connected paragraphs for explanations. Use lists for actual alternatives, steps, checks, or comparisons; avoid excessive headings, callouts, emphasis, inline code, or decorative separators.
- Use descriptive headings that name the topic or reader's question. Avoid hype and unsupported superlatives.
- After editing, read the article in order as a newcomer: What do I already know? Why does this section follow? Is each new term explained? Does the example still match? What conclusion can I safely draw?
- Check technical accuracy, repeated explanations, terminology, Markdown fences, image references, and navigation. Verify uncertain technical claims against primary documentation rather than polishing an inaccurate statement.

### Diagrams in Articles

- Use diagrams to clarify relationships, ownership, data flow, state changes, and ordering. Replace ASCII diagrams when a visual materially improves readability, not merely to add another image.
- Treat old generated images as subject-matter references, not geometry templates. Correct overlapping labels, oversized boxes, ambiguous containment, awkward arrows, and unnecessary empty space.
- Inline diagrams should not repeat the article heading in a large title or subtitle. Preserve meaningful component labels and interpretation-critical conditions inside the composition. Covers may keep a short title.
- Fit the canvas to the content after removing headings or other elements. Do not leave the vacated space above or below the diagram.
- When animation is requested, choose it only when it explains sequence, independent progress, or a state change. Keep comparisons and inventories static when motion adds no information. Preserve readable static fallbacks.
- Preserve existing diagram label language unless translation is requested. Keep original assets unless removal or replacement is explicitly requested.
- Follow `VISUAL_STYLE.md` for detailed visual and motion rules. Inspect final exports and representative animation frames, not only SVG source; verify that the article references the intended files.

## Visual Generation

When the user asks to create, edit, or propose a cover image, thumbnail, diagram, architecture visual, infographic, or technical illustration for this repository, read `VISUAL_STYLE.md` first and apply it by default.

Do this even when the user does not explicitly mention the style guide.

Use `VISUAL_STYLE.md` as the repository-wide visual direction for:

- blog post thumbnails;
- article series cover images;
- architecture diagrams;
- technical explainers;
- generated visual assets for posts.

For generated post thumbnails, prefer saving the final image as:

```text
images/image.png
```

Avoid overwriting existing images unless the user explicitly asks for replacement.
