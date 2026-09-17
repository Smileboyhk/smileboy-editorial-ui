---
name: smileboy-editorial-ui
description: Create concise, professional editorial diagrams for Smileboy's WeChat/public-account articles. Use for cognition models, business models, relationship maps, process diagrams, quadrant charts, stakeholder maps, ecosystem diagrams, role comparisons, and other explanatory visuals. The visual language should feel human-made in PowerPoint/Keynote: white background, deep blue, flat 2D geometry, sparse text, strong structure, restrained decoration.
---

# Smileboy Editorial UI Skill

## Purpose

Create article diagrams that communicate a concept in **3 seconds**.

The goal is not “beautiful AI infographic.” The goal is:

- simple
- professional
- human-made
- editorial
- easy to understand
- consistent across articles

Default mental model: **an experienced esports manager/coach drew the logic clearly in PowerPoint, then polished it lightly.**

---

## Core principle

> White background. Deep blue. Flat shapes. Few words. Strong structure. Weak decoration.

Every diagram must communicate **one core idea only**.

If a diagram needs paragraphs of explanation inside it, simplify it.

---

## Visual tokens

### Colors

Use these as defaults, not as mandatory exact values:

- Primary deep blue: `#234A84`
- Secondary blue: `#4F86D9`
- Light blue: `#DCE9F8`
- Very light background: `#F5F8FC`
- Main text: `#1F2937`
- Secondary text: `#6B7280`
- Divider / border: `#C8D6E8`
- Accent yellow-orange: `#F2B544`

Rules:

- Deep blue is the main identity color.
- Use the accent color **once or very sparingly** to highlight the key conclusion.
- Do not use rainbow palettes.
- Prefer white or very light gray backgrounds.
- Dark-background charts are exceptional, not default.

### Typography

Prefer clean Chinese sans-serif fonts available in the target environment.

Hierarchy:

- Figure title: bold, deep blue, concise
- Module title: bold / semi-bold
- Node text: regular or semi-bold
- Explanatory text: small, dark gray; avoid when possible

Text limits:

- Main title: ideally ≤ 12 Chinese characters
- Module label: ideally 2–6 characters
- Node label: ideally ≤ 8 characters
- Explanatory text: ideally 0–1 line

### Shapes

Prefer:

- circles
- concentric circles
- rectangles
- small-radius rounded rectangles
- simple arrows
- thin lines
- axes

Avoid:

- glossy cards
- oversized pill buttons
- 3D
- bevels
- glassmorphism
- neon
- gradients by default
- heavy shadows
- decorative illustrations
- excessive icons
- clip-art people

Use one border radius consistently.
Use one line weight consistently.

---

## Human-made feel

The design should not look algorithmically over-produced.

To create a human-made editorial feel:

1. Do not fill every empty area.
2. Keep generous white space.
3. Do not explain every node.
4. Avoid perfect decorative symmetry unless the model requires it.
5. Use alignment intentionally, but allow natural editorial spacing.
6. Prefer 4–7 meaningful labels over 15–25 tiny labels.
7. Make the reader understand the spatial relationship before reading details.
8. Do not add decorative slogans, footers, English labels, or corner ornaments unless explicitly requested.

---

## Default diagram families

Choose the simplest structure that expresses the idea.

### 1. Nested / ecosystem relationship

Use **Stakeholder Onion / concentric circles** when one entity belongs to progressively larger systems.

Example:

`职业选手 ⊂ 俱乐部 ⊂ 职业联赛 ⊂ 游戏生态`

Optional external stakeholders may be placed sparsely in the relevant ring, e.g.:

- 赛事方
- 赞助商
- 直播平台
- 媒体
- 游戏厂商
- 玩家社区

Do not add definitions in brackets unless required.

### 2. Cause / process

Use a **horizontal 3–5 step flow**.

Example:

`训练质量 → 比赛表现 → 成绩 → 职业价值`

Rules:

- 3–5 nodes preferred
- one-direction flow
- no decorative arrows
- highlight only the final or key node

### 3. Two-dimensional cognition model

Use **X/Y axes + quadrants**.

Example:

- X: 团队意识
- Y: 竞技能力

Use 3–4 labels in the field, not paragraphs.
Highlight the desired quadrant with the accent color.

### 4. Role / responsibility comparison

Use **two large boxes + simple relationship in the middle**.

Example:

`总教练 ↔ 教练`

Show only core responsibilities.
Prefer 3–5 bullets per side.

### 5. Components × relationship = result

Use when explaining that outcomes come from both elements and how they connect.

Structure:

`要素 × 连接关系 = 整体结果`

This is suitable for management systems, coaching systems, team operations, and organizational performance.

### 6. Simple hierarchy

Use stacked boxes or a clean tree when the relationship is primarily organizational or sequential.

Avoid complex org-chart spaghetti.

---

## Content selection rules

Before drawing, ask internally:

1. What is the single sentence this diagram should make obvious?
2. Which 3–7 labels are essential?
3. What can remain in the article text instead of the image?
4. What is the minimum structure needed to show the relationship?

Delete anything that does not help the main conclusion.

### Prefer

- concepts readers often misunderstand
- relationships that are hard to explain in prose
- hierarchy
- causality
- comparison
- position
- boundaries

### Avoid

- repeating entire article paragraphs
- long explanatory captions inside shapes
- obvious facts the reader already knows
- large lists of staff positions unless the article specifically discusses them

---

## Relationship with article text

The image should **not repeat the article**.

The article explains.
The image compresses.

Good image function:

- turn 300 words into one visual relationship
- create a memory anchor
- let readers understand the logic at a glance

Bad image function:

- duplicate every sentence from the article
- become a mini-poster with too many messages

---

## Rendering guidance

### For HTML / SVG

Prefer HTML/CSS or SVG for model diagrams when accurate text and geometry matter.

- Use real text, not rasterized AI-generated text.
- Keep layout deterministic.
- Use vector shapes.
- Export to PNG only at the end if needed.

### For image generation

Use image generation only when a designed visual is needed and exact text accuracy is not critical.
For diagrams with Chinese labels, prefer deterministic HTML/SVG/PPT rendering when possible.

### For article images

Default to landscape unless the content naturally requires portrait.
Maintain clear readability on mobile.
Do not use tiny text that disappears in WeChat preview.

---

## Quality checklist

Before final output, verify:

- [ ] One core idea only
- [ ] Understandable within ~3 seconds
- [ ] White / light background by default
- [ ] Deep blue visual identity
- [ ] Accent color used sparingly
- [ ] No unnecessary icons
- [ ] No gradients / glow / 3D by default
- [ ] No decorative footer / slogan unless requested
- [ ] Text is concise
- [ ] Labels are readable on mobile
- [ ] Alignment and spacing feel intentional
- [ ] Diagram feels like a human-made business/editorial slide, not an AI infographic

---

## Invocation examples

Users may invoke this skill by saying:

- “用 Smileboy Editorial UI 画这张图。”
- “按我的公众号 UI 风格做一个认知模型。”
- “用之前的简约商业图风格。”
- “按 Smileboy UI 做成同心圆 / 四象限 / 流程图。”

When invoked, apply this skill by default unless the user explicitly requests another style.

---

## Default response behavior

When the user asks for a diagram:

1. Identify the single core idea.
2. Choose the simplest diagram family.
3. Reduce content before drawing.
4. Use the standard visual tokens.
5. Prefer deterministic HTML/SVG/PPT for text-heavy diagrams.
6. Output the finished artifact or preview, not a long design explanation, unless the user asks for rationale.
