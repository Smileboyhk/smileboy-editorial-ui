# Smileboy Editorial UI Skill

Reusable visual-design skill for Smileboy's WeChat/public-account editorial diagrams.

## Main file

`SKILL.md`

## Typical invocation

- 用 Smileboy Editorial UI 画这张图。
- 按我的公众号 UI 风格做一个认知模型。
- 用之前的简约商业图风格。

## Recommended use

For Codex / agent workflows, place this folder in the skill directory supported by your runner and make `SKILL.md` available to the agent.

For ChatGPT conversations, upload/reference `SKILL.md` when needed. In the current project, the preference is also remembered, so saying “用 Smileboy Editorial UI” is enough to indicate this style.

## Included files

- `SKILL.md` — core design rules and invocation behavior
- `STYLE_TOKENS.json` — reusable visual tokens
- `EXAMPLES.md` — compact examples for common diagram families
- `examples/style-preview.html` — browser preview of the visual system
