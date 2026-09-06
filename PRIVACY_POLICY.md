Privacy Policy for AdShield Extra
Last Updated: September 2026

Introduction
AdShield Extra is committed to protecting your privacy. This Privacy Policy explains what information the extension processes and how it is used.

Information We Collect
AdShield Extra does not collect, store, transmit, or share any personal information about users.

Specifically, AdShield Extra does not:
- Collect personally identifiable information (PII)
- Track user activity or browsing behaviour
- Store or transmit browsing history
- Collect or read the content of any web page
- Create user profiles or analytics data

The extension's bundled filter lists are compiled at build time from public sources (GitHub-hosted filter-list repositories). No personal data, browsing history, or identifiers are ever included in the extension's own network activity.

How AdShield Extra Works
The extension registers its bundled and user-configurable filter lists with Chrome's native Declarative Net Request (DNR) engine. These rules block or allow third-party network requests based on those filter lists and on any custom rules you create yourself. All filtering happens entirely inside the browser — the extension never reads, inspects, or transmits the content of any request.

Cosmetic rules (hiding page elements) and scriptlet rules (small, targeted anti-fingerprinting or anti-annoyance scripts) are applied locally via Chrome's Scripting API, sourced only from: the extension's own bundled filter lists, rules you create yourself with the Cosmetic Element Picker, mitigations you select in the Privacy Inspector, or rules you import yourself via Manage Custom Rules. No rule content, page content, or browsing data ever leaves your device.

When you set a site's filtering mode from the popup (or add it to the Allow list), the extension updates the set of active DNR rules for that domain. Nothing is sent anywhere.

The Dynamic DNR filter panel works the same way: while it's open, it lists the third-party connections the current tab makes and lets you block or allow specific ones, per site. That per-site list is the same kind of local, on-device state as the per-site filtering mode above — see Data Storage below — and is never transmitted anywhere.

Worry-Free Safe Surfing (a temporary, opt-in protection boost you start yourself) and the Cookie Consent Clicker (which remembers a consent-button rule you create yourself, per site) also run entirely locally. Starting or ending a Worry-Free session, and any consent rule you create, are stored only on your device.

Third-Party Services
AdShield Extra does not use any third-party analytics, tracking, or advertising services. The extension's bundled filter lists are compiled from public GitHub-hosted sources at build time. All other processing happens locally within your browser using Chrome's built-in extension APIs.

Data Storage
The following data is stored locally on your device using chrome.storage.local:
- Your own custom filter rules (cosmetic and scriptlet), created via the Element Picker, Privacy Inspector, or Manage Custom Rules import
- Your per-site filtering mode (on/off/allowlisted)
- Your per-site third-party block/allow overrides (Dynamic DNR filter panel)
- Your own edited "familiar TLDs" list used by Worry-Free Safe Surfing's third-party-code/download protection
- Your Cookie Consent Clicker rules, per site
- Which built-in filter lists and Security & Privacy protections you have enabled or disabled
- Basic extension settings (e.g. whether tabs are auto-reloaded after a change)

None of this data is ever transmitted outside your browser.

Important Notice
AdShield Extra does not upload, transmit, or share:
- The content of any web page you visit
- Any request payload or response data
- Any personal data of any kind
- Your browsing history
- Any information about which websites you visit

Changes to This Privacy Policy
This Privacy Policy may be updated from time to time. Any changes will be reflected by updating the "Last Updated" date at the top of this document.

Third-Party Data Attribution
This extension bundles curated ad/tracking-network block lists (Kees1958, AdGuard, Disconnect, Peter Lowe's), an anti-adblock-circumvention list (AdGuard anti-adblock, Anti-Admiral), and cookie-consent-handling logic adapted from DuckDuckGo's autoconsent project, from Consent-O-Matic (CAVI, Aarhus University), and from Disconnect's own tracking-protection list — all used only for local, on-device filtering, never transmitted anywhere. Full attribution and license terms are in THIRD_PARTY_LICENSES.md.
