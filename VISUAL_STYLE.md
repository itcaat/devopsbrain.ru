# Visual Style Guide

Use this guide as a reusable reference for generated cover images, diagrams, and technical illustrations across the repository.

## Core Direction

Create minimalist technical visuals for an engineering blog.

The image should feel clear, structured, and useful rather than decorative. Prefer architecture diagrams, system flows, queues, timelines, dashboards, network paths, and component relationships over abstract tech backgrounds.

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
