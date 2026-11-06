# Custom Brand 404 Generator

A reusable Codex skill for designing and implementing brand-native 404 experiences. 根据品牌、产品、用户场景和现有架构，设计并实现真正可用的定制 404 页面。

## What it does / 能力

- Samples the target site and inspects the repository and existing 404.
- Derives 3–5 internal concepts, scores them and applies Anti-Template Tests.
- Selects recovery navigation and integrates with the current stack.
- Checks HTTP 404 behavior, links, assets, responsive layout and accessibility; fixes task-caused failures.
- Reports changes and explicitly labels unverified checks.

Execution is the default. “Preview only / 先给我方案 / 不要修改代码” produces a proposal without writing files. It does not deploy or modify production settings without authorization.

## Install / 安装

Download this repository, then copy the entire `custom-brand-404-generator` folder into a Codex skill directory on your computer. Keep `SKILL.md`, `agents`, `references`, `templates` and `examples` together. Use the skill directory supported by your Codex installation; an explicit file-path invocation also lets Codex read it without relying on automatic discovery.

You can ask Codex with the Skill Installer available:

> Use skill-installer to install the custom-brand-404-generator folder from this GitHub repository.

## Usage / 使用

Provide the website URL and the local project path (or say “current project”). Product, market, language and tone are optional. Codex derives missing nonessential details from the evidence.

```text
Use $custom-brand-404-generator.
Website: [your website URL]
Target project: [local project path or current project]
Page language: English
Analyze, choose a concept, implement, validate and repair. Do not ask me to choose between concepts.
```

Preview / 仅看方案:

```text
Use $custom-brand-404-generator.
Website: [your website URL]
Preview only. Do not create or modify any files.
```

中文示例:

```text
使用 $custom-brand-404-generator。
网站：[填写网站链接]
目标项目：[填写本地项目路径]
页面语言：英文
自行分析品牌与产品，选择方案，直接实现、验证并修复。
```

## Boundaries / 边界

A website URL alone does not provide its source repository. Without a target codebase, the skill completes a proposal and identifies the implementation blocker. If you want a new standalone demonstration, explicitly authorize creating it and name its output folder.

Correct HTTP status depends on framework and hosting configuration; a visual page alone cannot guarantee it. The skill must verify rather than assume. No mandatory new dependencies, analytics provider or i18n framework. No credentials are needed to install the skill, but live analysis and runtime validation depend on the tools available in your environment.

## Structure / 目录

```text
custom-brand-404-generator/
├── SKILL.md
├── agents/openai.yaml
├── references/
│   ├── discovery.md
│   ├── creative-framework.md
│   ├── experience-rules.md
│   ├── technical-integration.md
│   ├── analytics.md
│   └── validation.md
├── templates/
│   ├── execution-report.md
│   └── preview-report.md
└── examples/creative-examples.md
```

## Validation and limits / 验证与限制

Skill Creator quick validation and local reference checks passed during authoring. Website concepts were exercised in separate local demos. These are not guarantees of uniform behavior across models, frameworks or hosting providers. Demo websites, brand imagery and screenshots are deliberately excluded from this repository.

No third-party skill or plugin is required by name: the skill uses the web, file and preview capabilities available to the executing Codex environment. Brand assets used in a future website remain subject to their owners’ rights. This repository contains skill instructions, not those brand assets.
