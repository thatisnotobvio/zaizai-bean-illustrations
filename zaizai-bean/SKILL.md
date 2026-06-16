---
name: zaizai-bean
Description: Generates ZaiZai-style English text images. Used for user requests to generate "grotesque," "Little Brown," "hand-drawn," "text images," "product case studies illustrations," "image suggestions," "shot lists," and "remove titles/edit images" for English product case studies, UX writing, product strategy, user journeys, workflows, systems, roadmaps, frameworks, decision-making, metrics, and product thinking. The default style uses the ZaiZai Bean IP, pure white hand-drawn illustrations, minimal red, orange, and blue annotations, and a clean, simple yet imaginative visual style and system-based storytelling.
---

# ZaiZai Bean (with accompanying images)

## Core positioning

Design and generate 16:9 landscape illustrations for English Product case-studies for design portfolios. The goal is not to create commercial illustrations, SaaS marketing graphics, UI mockups, PowerPoint infographics, or cute cartoons, but to transform product decisions, user insights, workflows, systems, structures, tradeoffs, roadmaps, metrics, and strategic thinking into clean, quirky, creative, readable, but not instructional, hand-drawn explanatory diagrams.

The default visual IP is "ZaiZai Bean":solid brown, white dotted eyes, thin legs, and an empty expression, earnestly doing something slightly absurd but completely logical. ZaiZai Bean must participate in the core actions of the image, and cannot just stand by as decoration.

## Read these references first

Read only as needed for the task; do not fill the entire context at once.
- Style DNA, colors, text, tabos.
- The image, personality, action library, and taboos of the ZaiZai Bean IP.
- Structure type, original metaphor method and iterative engraving rules.
- Template for prompts for single raw images.
- Post-generation inspection and iteration rules.
- Perform only low-frequency visual calibration and do not enter the default generation path. Do not copy the composition, objects, or annotations of these examples.

## Workflow

### 1. Digest the main text
First, read the content provided by the user, including the main text, links, case-studies, Markdown files, Notion Pages, screenshots or product document. Extract the key points:
- What is the core insight?
- Which paragraphs represent cognitive shifts?
- What content is suitable for explanation with pictures?
- Where are text-only text options suitable, and images not needed?

Avoid using images evenly. Prioritize "cognitive anchors," such as: core decisions, tradeoffs, user pain points, user journeys, prioritization logic, feedback loops, product frameworks, system bottlenecks, information flow, before-and-after transformations, multi-step processes, product strategy shifts, common pitfalls, and changes in character status.

### 2. Image-first strategy
If the user simply ask for "analysis on how to choose images/thinking about where images are needed," provide a shot list first. Clearly describe each image:
- After which paragraph?
- The theme of the picture
- core meaning
- Structure type
- What is ZaiZai Bean doing in the picture?
- Suggested elements
- Suggested English annotation words
The default is 4-8 pages. For every short case studies, use 1-3 pages; for long case studies, don't easily exceed 9 pages. Just use enough to avoid turning the main text into a picture album.

### 3. Single-page generation
If the user explicitly requests "Generate/Output/Create Image/Generate for Me", do not stop and wait for confirmation; use the built-in function `image_gen` to generate each image separately. Do not combine multiple images into one.
Each diagram should illustrate only one core structure. The prompt must include:
- 16:9 English Chinese Text with Images
- pure white background
- Brown hand-drawn line art
- A small number of red/orange/blue handwritten English annotations
- Ample white space
- ZaiZai Bean is the core action subject.
- Product Designer and Product Manager mindset
- Product thinking metaphor
- PPT presentations, commercial illustrations, childish or cute designs, complex structures, and top-left corner headings are prohibited.

Do not replicate past examples. Examples only provide style density and how ZaiZai Bean (the author) participates; do not directly reuse existing compositions such as "conveyor belt breakpoints/ZaiZai Bean line drawing/material fish/stamp toolbox/common pitfall paths," unless the user explicitly requests a specific image to be replicated. Do not reinvent a strange but valid metaphor from the current case study each time.

### 4. Inspection and Iteration
After generating, check `references/qa-checklist.md`. If the following problems occur, prioritize regenerating or partially editing:
- The little brown thing is just for decoration.
- The screen is too full.
- Too much like a flowchart/PPT
- Too much English or serious spelling errors
- The top left corner displays titles such as "Common Pitfalls/Flowcharts/System Architecture Diagrams".
- The art style is too cute, childish, and rigid.
- The background is not a clean white background.

### 5. Save delivery
If the user is working within the workspace, copy the final diagram to:

```text
assets/<case-study-slug>-illustrations/
```

Name in order:

```text
01-topic-name.png
02-topic-name.png
```

Retain the original generated files and do not overwrite existing assets unless the user explicitly requests a replacement.

## Output diameter

The strategy output before generation should be short and accurate. The delivery after generation should include:
- Several images were generated
- Purpose of each image
- Save path
- Which charts are the most stable, and which are optional?

Avoid lengthy explanations of style theory; let the images speak for themselves.
