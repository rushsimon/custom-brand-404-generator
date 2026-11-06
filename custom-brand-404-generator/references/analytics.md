# Existing analytics integration only

Inspect existing GA4, GTM/dataLayer or analytics abstractions and consent rules. Add events only when the existing pipeline supports them and they answer a useful recovery question. Do not install GA4 or a second analytics SDK for the 404. If infrastructure is absent or unsuitable, report no events added.

Possible event names (map to project conventions): 404_page_view, 404_navigation_click, 404_search and 404_recommendation_click. Possible parameters: broken_url, referrer, destination_url, link_type, search_term and recommendation_type. Include only useful safe parameters; they are not a required schema.

Normalize broken/destination URLs to safe same-site paths; omit query strings, fragments, credentials and token-like or personal path segments. External referrers should be reduced to origin/domain if permitted. Do not collect raw search text by default; prefer search usage or a nonsensitive category unless an existing approved sanitization policy permits more. Never send sensitive information or bypass consent.

Determine who already owns page-view emission. A custom 404 event must not trigger an extra normal page view; avoid duplicate registration/firing on hydration, rerenders, client navigation, development strict mode or repeated event bindings. Follow the project's lifecycle/deduplication patterns. Click handlers must not delay or block navigation.

Verify using local mocks, debug hooks or event inspection without intentionally polluting production analytics. Verify one event per intended action and correct sanitized parameters. Report event names, parameters and implementation method, or the reason tracking was omitted. Distinguish code inspection from observed event delivery.
