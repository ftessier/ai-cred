# The ai-cred framework — A simple standard for human-ai attribution

`ai-dr-cr`

## Table of contents <!-- omit in toc -->

- [1. Purpose](#1-purpose)
- [2. Format](#2-format)
- [3. Contribution codes](#3-contribution-codes)
- [4. Common examples](#4-common-examples)
- [5. Attribution layers](#5-attribution-layers)
- [6. Usage guidelines](#6-usage-guidelines)
- [7. Responsibility](#7-responsibility)
- [8. License](#8-license)

## 1. Purpose

The **ai-cred** framework provides a simple, universal way to declare the respective contributions of humans and AI systems in creating a work. Like Creative Commons for copyright, it scales from a quick shorthand to detailed attribution statements.

## 2. Format

```
ai-[human contribution]-[ai contribution]
```

## 3. Contribution codes

All codes use only the letters **c, r, e, d** — easy to remember as "cred" (credibility, as in the expression "street cred").

| Code | Level | Meaning                                                               |
| ---- | ----- | :-------------------------------------------------------------------- |
| `no` | 0     | **No involvement** — absent or only trivial tools (e.g., spell-check) |
| `re` | 1     | **Reviewed** — checked, approved, responded, minor corrections        |
| `ed` | 2     | **Edited** — substantially revised or rewrote                         |
| `dr` | 3     | **Directed** — guided, prompted, shaped the work                      |
| `cr` | 4     | **Created** — produced the original content                           |

The scale reflects intensity of contribution: `no` < `re` < `ed` < `dr` < `cr`

## 4. Common examples

| Tag        | Human    | AI       | Typical Scenario                                  |
| :--------- | :------- | :------- | :------------------------------------------------ |
| `ai-cr-no` | Created  | None     | Fully human-authored, no AI involved              |
| `ai-cr-re` | Created  | Reviewed | Human wrote it, AI checked grammar                |
| `ai-cr-ed` | Created  | Edited   | Human wrote it, AI polished style                 |
| `ai-cr-dr` | Created  | Directed | AI guided structure, human produced content       |
| `ai-ed-cr` | Edited   | Created  | AI drafted, human substantially rewrote           |
| `ai-dr-cr` | Directed | Created  | Human prompted and curated, AI generated          |
| `ai-re-cr` | Reviewed | Created  | AI generated, human approved with minimal changes |
| `ai-no-cr` | None     | Created  | Fully AI-generated                                |

## 5. Attribution layers

**Short form** — minimal inline reference:

```
ai-dr-cr
```

**Standard form** — includes tool:

```
ai-dr-cr | Claude Opus 4.5
```

**Extended form** — full disclosure statement:

```
ai-dr-cr | Claude Opus 4.5 (Anthropic) | February 2025

The author provided detailed prompts, source materials, and structural
guidance. AI generated the initial draft. The author reviewed and
curated the output, making selective edits for accuracy and tone.
The author takes full responsibility for the final content.
```

## 6. Usage guidelines

1. **Be accurate** — choose codes that honestly reflect the work process
2. **When in doubt, disclose more** — use the extended form for complex cases
3. **Mixed works** — for works with distinct sections, attribute separately: `Text: ai-cr-ed | Images: ai-dr-cr`
4. **Evolving works** — update attribution if the human-AI balance changes in revisions
5. **Tool specificity** — name the AI system when known; use "ai" generically if multiple or unknown

## 7. Responsibility

The **ai-cred** framework describes *process*, not *accountability*.

The human contributor always bears responsibility for the final work's accuracy, ethics, and fitness for purpose — regardless of AI involvement level.

## 8. License

The AI-CRED Framework is released under **CC0 1.0 Universal (Public Domain)**.

You may freely use, adapt, and build upon this framework without restriction.
