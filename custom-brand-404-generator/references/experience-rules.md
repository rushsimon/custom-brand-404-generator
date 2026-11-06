# Recovery, expression and localization

## Useful before promotional

Make “what happened” and “what next” immediately clear, with at least one prominent verified recovery path. Choose a small relevant set of home, category, docs, contact, search or content links. Never mechanically include all modules.

- Home must use the correct deployment base and locale.
- Back is optional and needs a reliable home fallback when no useful same-site history exists; do not make it the only exit.
- Search requires an existing working search endpoint/component, a label, submit behavior and empty/error handling. If unavailable, omit it rather than add a decorative input.
- Recommendations must come from actual known routes/content. Only label content “best seller”, “popular” or an offer when supported by evidence. Do not fabricate discounts or reviews.
- Optional typo suggestions may compare the sanitized path against a bounded inventory of real same-site routes. Escape output, cap work, omit low-confidence matches and never force a redirect. No speculative URL generation or arbitrary outbound destinations.

Commerce/affiliate links, quotes, signup and pricing are secondary to recovery. Match site type without turning the error into an aggressive landing page.

## Assets and motion

1. Reuse approved local brand/product imagery, icons and components first. Confirm file existence, rights/context and suitable resolution; do not hotlink arbitrary assets.
2. Build meaningful new visuals with scoped HTML/CSS/SVG/gradients and lightweight motion.
3. If essential imagery remains unavailable, supply an image-generation prompt describing brand style, palette, product, composition, lighting, mood, aspect ratio, background and intended usage. Keep a complete functional fallback. Do not make delivery depend on an ungenerated image or claim it exists. Generate only when requested/authorized and supported by available tools.

Do not fill space with unrelated stock photos, 3D objects or illustrations. Set dimensions/aspect ratios; use existing font assets and loading conventions.

Use hover, pointer movement, animation, drag, easter eggs or a small game only if brand appropriate, performant and useful or delightful. Core navigation must remain visible and independent of interaction completion, pointer input and JavaScript effects. Provide keyboard/touch equivalents where relevant. Prefer CSS/SVG or existing libraries; reduce intensity if costly.

## Copy and localization

Generate all displayed headline, support text, CTA, search placeholder/labels, recommendations, microcopy, interaction and error states in the existing site's voice. Match vocabulary, sentence length, capitalization and humor. Make the missing-page meaning unambiguous even with a metaphor. Never imply an actual product fault or service outage without evidence.

For a single-language site use its language. For multilingual sites reuse existing locale resolution, translation files, components, fallback rules and routes. Cover locales exposed by the changed route; adjust humor, terminology, CTA and cultural expression rather than translating mechanically. Do not introduce a parallel i18n framework or break locale on recovery links. An explicit requested page language overrides the detected language. Target market alone informs localization but does not authorize replacing the existing site language or locale architecture.

## Accessibility and responsive quality

Use semantic landmarks, a clear heading hierarchy, actual links for navigation, buttons for actions, labeled forms, visible focus and meaningful alt text (empty alt for decoration). Use ARIA only to fill semantic gaps. Check contrast, keyboard order, focus behavior, touch targets and zoom/overflow. Respect prefers-reduced-motion with a static/reduced alternative; motion must not carry essential meaning. Keep mobile, tablet and desktop density consistent with the site's design system.
