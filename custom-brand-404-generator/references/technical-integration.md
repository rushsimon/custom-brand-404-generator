# Native implementation and code safety

## Plan the smallest integration

Inspect the actual installed framework version and routing/deployment configuration. Reuse header/footer/layout, container, buttons, cards, typography, icons, search, product cards, tokens and analytics where available. Respect server/client component boundaries. Avoid duplicate shell elements if the framework already wraps the not-found component. Scope new styles to the page; preserve unrelated working tree edits.

Typical entrypoints are discovery hints, not recipes: Next.js app not-found.tsx or pages/404.tsx; static 404.html; WordPress active theme 404.php; Shopify theme templates supported by its current version; Astro/Nuxt platform-native not-found handling; React router fallback plus host/server handling. Read project conventions and appropriate current official docs when unfamiliar. Do not install a new stack or rewrite the router to make an example fit.

No unrelated refactors, dependency upgrades, global CSS side effects, deletion of existing features or large UI frameworks. Default to no new dependencies. Consider one only if existing capabilities cannot meet a concrete requirement and the benefit outweighs cost; explain it in the audit and follow existing authorization constraints.

## HTTP correctness is a deployment property

Use the native not-found mechanism and the existing host/adapter's error handling. Test a genuinely nonexistent path via a direct request and refresh, including a nested path, not just /404 or client navigation. A designed error screen alone does not prove status correctness.

Require an actual HTTP 404 response for missing documents. Do not redirect every missing URL to a 200 home page or /404 page. A correct-looking SPA catch-all returned as HTTP 200 is still a soft 404. Static hosts need their supported error-document behavior; pure client routing cannot set the initial HTTP response. Streaming frameworks can send headers before rendering a missing-page component, so verify actual production-mode responses rather than assuming a filename guarantees status. Where needed, resolve missing resources before response streaming using a supported mechanism.

If host/server control is absent, avoid false fixes: keep useful page integration, state the HTTP blocker and supply the smallest required hosting change. Do not mark the HTTP gate passed until measured. No SEO keyword blocks, hidden text, invented content or ranking-oriented long copy; metadata/robots directives never substitute for correct status.

## Runtime resilience

Keep assets valid under nested missing URLs and configured base paths; use framework asset helpers or appropriate root/base URLs. Avoid expensive queries and unnecessary network calls on every error. Bound any suggestion computation. Escape untrusted path/search values and avoid unsafe HTML or open redirects. A missing product/resource must not crash the 404 itself; provide a simple static recovery fallback when optional data is unavailable.

Reserve visual dimensions, avoid heavy images/JS and reuse existing font and caching strategy. Keep functional navigation server-rendered where supported, with lightweight progressive interaction. Preserve locale and existing consent behavior.

Maintain an audit as work proceeds: files added/modified, dependency changes, assets added, routes changed and tracking changes, each with a reason. Report none explicitly where applicable.
