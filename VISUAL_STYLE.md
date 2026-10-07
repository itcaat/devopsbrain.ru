# Visual Style Guide

Use this guide as a reusable reference for generated cover images, diagrams, and technical illustrations across the repository.

## Core Direction

Create minimalist technical visuals for an engineering blog.

The image should feel clear, structured, and useful rather than decorative. Prefer architecture diagrams, system flows, queues, timelines, dashboards, network paths, and component relationships over abstract tech backgrounds.

## Default Technical Diagram Style

Use the visual language of this reference as the default for technical diagrams and diagram-based article covers:

```text
content/posts/2026-08-06-kafka-from-zero-to-hero-part-1/images/kafka-overview.svg
```

The default style is a clean editorial architecture canvas:

- 3:2 landscape composition on a light off-white background;
- a very subtle dot grid that supports alignment without competing with content;
- a large, left-aligned title with one or two important words highlighted in dark red;
- a short subtitle listing the main concepts covered by the visual;
- an optional compact dark badge in the upper-right corner for context or scope;
- one clear technical composition beneath the title, organized from left to right;
- related components grouped inside labeled system boundaries;
- dark navy section headers, dark red primary flows, and muted blue or green secondary flows;
- rectangular nodes with modest corner radii, thin borders, restrained shadows, and generous internal padding;
- short English labels inside diagrams unless the user requests another language;
- a compact dark summary or legend strip at the bottom when it helps explain the visual hierarchy.

Technical accuracy takes priority over visual symmetry. Show ownership and containment explicitly: for example, a Kafka Partition belongs inside a Kafka cluster and is hosted on a Broker rather than appearing as an unrelated stage in a linear pipeline.

Keep the diagram readable at thumbnail size. Prefer a few meaningful components and visible relationships over a complete inventory of the system.

### Motion Policy

Generate static SVG and PNG assets by default. Add GIF or SVG animation only when the user explicitly requests animation.

When animation is requested:

- keep nodes, labels, containers, and the camera stationary;
- animate only meaningful system behavior such as event flow, replication, processing, retries, or offset progress;
- use small particles or compact markers that follow existing routes;
- keep loops calm, deterministic, and seamless;
- do not add decorative motion, pulsing backgrounds, or moving text;
- always provide a readable static PNG frame alongside the animated asset.

## Visual Language

- Light off-white background.
- Charcoal or near-black primary text.
- One strong dark red accent.
- Muted blue and muted green accents for secondary nodes.
- Thin lines, clean arrows, and simple geometric blocks.
- Vector-like bitmap rendering.
- Generous spacing and readable hierarchy.
- Rectangular diagram nodes with modest corner radius.
- Clear labels and legible typography.

## Composition

- Default aspect ratio: 3:2 landscape.
- Make the subject readable as a blog thumbnail.
- Use a strong title or topic label when text is required.
- Keep diagrams centered and balanced.
- Prefer a simple flow from left to right or top to bottom.
- Use grouped areas for related concepts, such as producers, brokers, partitions, consumers, databases, queues, or services.

## Diagram Layout Quality

- Center labels and icons as a single visual group inside each node. Do not align every label from a fixed left inset when label lengths differ.
- Keep service/node icons close to text scale. As a rule of thumb, icon boxes should be about the height of a capital letter or only slightly larger, not dominant pictograms inside text-heavy nodes.
- For horizontal `icon + label` groups, center the full group within the rectangle and keep consistent spacing between the icon and text.
- Vertically center the full `icon + label` group inside the node, not just the icon or the text independently.
- Size every text container from the rendered text, not from a rough estimate. Leave visible horizontal padding on both sides, especially for callouts, captions, and footer notes.
- When drawing SVG text, remember that `y` usually positions the text baseline rather than the visual center. Prefer explicit visual checks after export, and avoid relying on `dominant-baseline` unless the renderer is known to handle it consistently.
- Export and inspect the final raster image before accepting the asset. Check that text is not drifting up/down, icon-label groups are centered, arrows point to node centers, container boxes fully enclose their text with padding, and all labels remain readable at thumbnail size.

## Avoid

- Busy backgrounds.
- Stock-photo style imagery.
- People, mascots, and fictional characters unless explicitly requested.
- Logos or brand marks unless explicitly requested and legally appropriate.
- Watermarks.
- Random code snippets as decoration.
- Dark blurred server rooms.
- Decorative gradient blobs, bokeh, or abstract neon fog.
- Tiny labels that will not survive thumbnail scaling.
- Overly complex diagrams with too many elements.

## Reusable Prompt Base

```text
Create a minimalist technical blog visual in the repository style: clean off-white background, charcoal text, one dark red accent, muted blue and green secondary accents, thin architecture-diagram lines, simple geometric nodes, generous spacing, vector-like bitmap rendering, professional engineering blog aesthetic. Make it readable as a thumbnail. No clutter, no people, no mascots, no logos, no watermark, no decorative gradient blobs.
```

## Example Use

```text
Create a 3:2 cover image for an article about Kafka consumer lag using the repository visual style. Show a simple flow from Producer to Topic Partitions to Consumer Group, with one partition visibly lagging behind. Use clean labels, thin arrows, off-white background, charcoal text, dark red accent, and muted blue/green nodes.
```

## Text Handling

When an image needs text:

- Keep text short.
- Provide exact text in the prompt.
- Avoid long sentences inside the image.
- Prefer 1 title plus 3-5 labels.
- Verify generated text carefully before using the image.

## File Naming

Store every visual asset for an article in the `images/` subdirectory of that article:

```text
content/posts/<post-slug>/images/
```

This applies to thumbnails, diagrams, illustrations, animated GIFs, static PNG fallbacks, and editable SVG sources. Do not place visual assets next to `index.md`.

Keep related formats together and use the same descriptive basename:

```text
images/kafka-log-offsets.svg
images/kafka-log-offsets.png
images/kafka-log-offsets.gif
```

Avoid additional preview or generated-asset subdirectories unless the user explicitly requests them.

For post thumbnails, prefer:

```text
images/image.png
```

For additional generated diagrams inside a post, prefer descriptive names:

```text
images/consumer-lag-flow.png
images/partition-rebalance.png
images/replication-isr.png
```
