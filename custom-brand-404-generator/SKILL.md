---
name: custom-brand-404-generator
description: Create, redesign or improve a custom branded 404 / Not Found page using website, brand, product and current-project evidence; implement by default or provide a design-only preview when requested. 适用于定制404页面、重新设计404页面、品牌产品创意Not Found页面。 Not for ordinary page design, landing pages or general website redesign without a 404-specific request.
---

# Custom Brand 404 Generator

Create a 404 experience that feels intentionally designed by the target brand. Default to completing analysis, selection, implementation, validation, fixes and a concise report in one run. Do not ask the user to approve concepts or routine implementation choices.

## Input and mode

Accept a website URL plus optional product, audience, market, tone and constraints. Infer missing nonessential context from the project and sampled website. If no URL is supplied, use a project-configured canonical origin; otherwise proceed from local evidence and disclose limited live research. Ask only for an indispensable missing target or authorization that cannot be inferred.

- **Execution (default):** modify the identified target project and validate it.
- **Preview:** explicit instructions such as “先给我方案”, “不要修改代码”, “只做设计”, “Preview only” or “Don't implement yet”. Perform read-only analysis and concept selection; deliver a design proposal without creating or modifying files, installing packages or running commands that generate output files. Keep analysis and the proposal in the conversation; read-only tool access is allowed. Proposal details may describe recovery, assets, motion and localization; do not execute them.

Use explicit user input > current project context > live website > inference for facts. Repository architecture governs implementation. Use the live site's visual system as the default visual reference unless explicit user input or current project requirements override it; report material differences.

Treat technical correctness and usable recovery as mandatory gates. Among viable solutions prioritize usability, brand consistency, creativity, conversion, then visual complexity. Never trade correct HTTP status or a clear escape route for a concept.

## Workflow and reference loading

Load each reference only when its stage or condition applies; do not preload the entire folder. Discovery and creative selection are shared by both modes. Execution additionally needs experience, technical integration and validation; analytics and examples are conditional. Reuse already-read guidance during repair rather than reloading it.

1. **Analyze the target, inspect repository and existing 404.** Read [discovery](references/discovery.md). Establish the requested website from the URL/homepage or local site context, then identify the intended repository, stack, deployment, existing not-found route and reusable components before edits. Inspect existing 404 behavior and decide to improve or rebuild with a reason.
2. **Understand the website.** Follow discovery's adaptive sampling and evidence ledger. Establish site type, brand, product behaviors, audience, design system and language. Do not crawl the whole site. Use available web/browser tools under the active environment's rules; unavailable access is a disclosed limitation, not permission to invent evidence.
3. **Generate and choose.** Read [creative framework](references/creative-framework.md). Produce 3–5 distinct internal concepts, evaluate each, apply all Anti-Template Tests and select one. Read [creative examples](examples/creative-examples.md) only if useful to understand derivation; never use them as a concept catalog. Show only the winner unless multiple concepts are requested.
4. **Preview branch.** Read only the applicable recovery, expression and localization sections of [experience rules](references/experience-rules.md) to ground the proposal; read [technical integration](references/technical-integration.md) only if a concrete routing/status question needs resolution. Stop implementation here and use [preview report](templates/preview-report.md). Describe how the selected concept would work and its validation plan. Never claim an implemented page.
5. **Implement.** Read [experience rules](references/experience-rules.md) and [technical integration](references/technical-integration.md). Choose recovery features, secondary conversion, interaction intensity, assets and localization based on evidence. Reuse existing components and make the minimum necessary change. Read [analytics](references/analytics.md) only when existing analytics can support useful events.
6. **Verify and fix.** Read [validation](references/validation.md). Run relevant available checks, test the actual missing URL and repair task-caused failures, then retest affected checks. Do not claim unperformed checks passed.
7. **Deliver.** Use [execution report](templates/execution-report.md), with a file/change audit and honest verification results. Detailed analysis and scoring are optional only when requested.

## Execution boundaries

A URL authorizes analysis, not edits to an unrelated current folder. If no target repository is identifiable, finish the selected proposal and implementation plan, explicitly state implementation is blocked, and ask for the target path; do not silently switch modes or create a substitute app. If source is available but hosting status behavior cannot be controlled locally, implement the appropriate native integration and report the remaining hosting blocker without claiming completion.

Do not deploy, publish or modify production settings unless authorized. Keep unrelated user changes intact. Do not add dependencies by default, copy competitors, invent links/products/offers or introduce a new analytics/i18n framework. Avoid progress questions when reasonable decisions can be made from evidence.

## Extending the skill

Shared rules live in the references above. Add a site-type or stack reference only when it contains decisions not covered there; link it from discovery or technical integration and read it only for matching projects. Keep examples explanatory and report templates structural. Never add a shared page layout or category-to-concept lookup table.
