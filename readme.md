# cred — A memorable standard for Human-AI attribution <!-- omit in toc -->

[![cred](https://img.shields.io/badge/cred-dr--cr_1.0-red)](https://github.com/ftessier/cred)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)

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

The **cred** standard provides a simple, universal way to declare human and AI contributions in creating a work. Inspired by [Creative Commons](https://creativecommons.org/) for copyright, it scales from quick shorthand to detailed attribution. The system is voluntary and trust-based: there is no oversight or legal enforcement. The goal is to give authors a standard way to label AI involvement for transparency, including an unambiguous signal when no AI was used (`cred-cr-no`).

## 2. Format

```text
cred-[human contribution]-[ai contribution] [version]
```

## 3. Contribution codes

All codes use only the letters **c, r, e, d** — easy to remember as "cred" (meaning _credits_, _credentials_ or _credibility_).

| Code | Level | Meaning                                                               |
| ---- | ----- | :-------------------------------------------------------------------- |
| `no` | 0     | **No involvement** — absent or only trivial tools (e.g., spell-check) |
| `re` | 1     | **Reviewed** — checked, approved, responded, minor corrections        |
| `ed` | 2     | **Edited** — substantially revised or rewrote                         |
| `dr` | 3     | **Directed** — guided, prompted, shaped the work                      |
| `cr` | 4     | **Created** — produced the original content                           |

The scale reflects intensity of contribution: `no` < `re` < `ed` < `dr` < `cr`

## 4. Common examples

Badge colors indicate primary authorship at a glance: green when the human created the core content, red when AI created it, and yellow for balanced collaboration.

| Tag                                                                                              | Human    | AI       | Typical Scenario                                  |
| :----------------------------------------------------------------------------------------------- | :------- | :------- | :------------------------------------------------ |
| [![cred](https://img.shields.io/badge/cred-cr--no_1.0-green)](https://github.com/ftessier/cred)  | Created  | None     | Fully human-authored, no AI involved              |
| [![cred](https://img.shields.io/badge/cred-cr--re_1.0-green)](https://github.com/ftessier/cred)  | Created  | Reviewed | Human wrote it, AI contributed minor changes      |
| [![cred](https://img.shields.io/badge/cred-cr--ed_1.0-green)](https://github.com/ftessier/cred)  | Created  | Edited   | Human wrote it, AI polished style                 |
| [![cred](https://img.shields.io/badge/cred-cr--dr_1.0-green)](https://github.com/ftessier/cred)  | Created  | Directed | AI guided structure, human produced content       |
| [![cred](https://img.shields.io/badge/cred-cr--cr_1.0-yellow)](https://github.com/ftessier/cred) | Created  | Created  | Iterative collaboration, balanced contribution    |
| [![cred](https://img.shields.io/badge/cred-ed--cr_1.0-red)](https://github.com/ftessier/cred)    | Edited   | Created  | AI drafted, human substantially rewrote           |
| [![cred](https://img.shields.io/badge/cred-dr--cr_1.0-red)](https://github.com/ftessier/cred)    | Directed | Created  | Human prompted and curated, AI generated          |
| [![cred](https://img.shields.io/badge/cred-re--cr_1.0-red)](https://github.com/ftessier/cred)    | Reviewed | Created  | AI generated, human approved with minimal changes |
| [![cred](https://img.shields.io/badge/cred-no--cr_1.0-red)](https://github.com/ftessier/cred)    | None     | Created  | Fully AI-generated                                |

## 5. Attribution layers

**Short form** — minimal inline reference:

```text
cred-dr-cr 1.0
```

**Standard form** — includes tool:

```text
cred-dr-cr 1.0 | Claude Opus 4.5
```

**Extended form** — full disclosure statement:

```text
cred-dr-cr 1.0 | Claude Opus 4.5 (Anthropic) | February 2026

The author provided detailed prompts, source materials, and structural
guidance. AI generated the initial draft. The author reviewed and
curated the output, making selective edits for accuracy and tone.
The author takes full responsibility for the final content.
```

## 6. Usage guidelines

1. **Capture** — choose codes that honestly reflect the work process
2. **Refine** — attribute distinct parts separately (e.g. `Text: cred-cr-ed 1.0 | Images: cred-dr-cr 1.0`)
3. **Evolve** — update attribution as works and contributions change
4. **Disclose** — reveal more for complex or uncertain cases

## 7. Responsibility

The **cred** standard describes *process*, not *accountability*. The human contributor always bears responsibility for the final work's accuracy, ethics, and fitness for purpose — regardless of AI involvement level.

## 8. License

The **cred** standard is released under [**CC0 1.0 Universal (Public Domain)**](https://creativecommons.org/publicdomain/zero/1.0/legalcode.en). You may freely use, adapt, and build upon this standard without restriction.
