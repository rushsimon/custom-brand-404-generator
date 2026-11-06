# Validate, repair, revalidate

Use available project commands and actual route behavior. Record each check as Passed, Failed or Not Verified with brief evidence; a checklist is not evidence by itself. Do not turn unavailable tooling into an assumed pass.

## Checks

| Area | Required evidence where runnable |
| --- | --- |
| Routing/status | Direct requests to unique nonexistent top-level and nested paths return 404; refresh works; native missing-resource flow works; real routes still work. Check locale/base-path variants when relevant. Separate development from production/preview/host behavior. |
| Recovery | Activate each changed CTA/link; confirm real destinations, working search and accurate suggestions; back fallback works. Verify source inventories when runtime unavailable, labeling that limitation. |
| Assets | Images/fonts/SVG load without missing requests; deep-path asset URLs work. |
| Frontend | Run relevant build/type/lint/test commands that exist. Inspect console/network for task-caused errors, hydration problems and broken imports. |
| Responsive | Inspect representative mobile (~375px), tablet (~768px) and desktop (~1440px), adjusting to site breakpoints; check overflow, density, legibility, wrapping and touch navigation. |
| Accessibility | Keyboard navigation, visible focus, labels/semantics, contrast, alt text and reduced-motion behavior. Automated checks supplement manual inspection. |
| Performance | Inspect new asset/JS cost, unnecessary requests and layout shifts; no unsupported claim of measured Core Web Vitals. |
| Analytics | If added, check event count, consent and sanitized parameters; no duplicate normal page view or unintended firing. |
| Scope/design | Review diff for accidental global changes, unsupported claims and needless dependencies; rerun the Anti-Template Tests on the actual result. |

Where tools permit, capture page screenshots for visual inspection. Do not claim visual responsiveness or console checks from a successful build alone. Use a preview server without deploying unless deployment was separately authorized.

## Repair loop

Fix task-caused build/import/asset/route/console/layout failures, rerun the failed checks and affected checks, and update their results. Separate preexisting failures from introduced ones using available baseline evidence; do not rewrite unrelated code just to clean a baseline.

Continue while a concrete, permitted fix is available. If repeated targeted attempts make no meaningful progress (normally reassess after three), or the fix requires inaccessible credentials, hosting control or an unrelated migration, stop that repair path, preserve reviewable work and report the exact blocker. Never bypass a check or weaken correct status requirements to mark completion.

## Final acceptance

Answer internally: native to brand? concept tied to product/scenario? meaningful without logo? interchangeable across ten competitors? clear quick recovery? actual HTTP 404? components reused? unnecessary dependencies avoided? implementation verified? scope minimal?

The competitor answer should be No; other quality questions should be Yes with evidence. Unmet correctness/recovery gates mean delivery is incomplete/blocked, even if code was written. For partial verification, say exactly what is Not Verified and why; do not label the overall page fully validated.
