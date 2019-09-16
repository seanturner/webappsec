# WebAppSec @ TPAC 2019

Sept. 17th and 19th, 8:30 - 18:00 at the [Hilton Fukuoka Sea Hawk](https://www3.hilton.com/en/hotels/japan/hilton-fukuoka-sea-hawk-FUKHIHI/index.html).

## Sept. 17th

* 9:00 - 9:30 - Introductions, problem statements, framing the next day and a half.
* 9:30 - 10:00 - [Something california-friendly, e.g. `Sec-Origin`]
* 10:00 - 10:30 - Continuous specification (plh@, wseltzer@)
* 10:30 - 11:00 - ☕ Coffee
* 11:00 - 12:00 **CSRF / 👻Spectre👻 / XSLeaks**
  * [Fetch Metadata](https://github.com/w3c/webappsec-fetch-metadata)
  * COOP/[CORP](https://fetch.spec.whatwg.org/#cross-origin-resource-policy-header)/[COEP](https://github.com/mikewest/corpp)
  * Double-keyed (or more) caches
* 12:00 - 12:30 - Networky things
  * [MIX2](https://w3c.github.io/webappsec-mixed-content/level2.html)
  * HSTS: [Apple's mitigations](https://webkit.org/blog/8146/protecting-against-hsts-abuse/), (Strict-Navigation-Security](https://github.com/mikewest/strict-navigation-security)
  * Intranet / Internet: [CORS-RFC1918](https://wicg.github.io/cors-rfc1918/)
* 12:30 - 13:30 - 😋 Lunch 😋
* 13:30 - 14:30 - Authentication
  * [`IsLoggedIn` API](https://lists.w3.org/Archives/Public/public-webappsec/2019Sep/0004.html) ([@johnwilander](https://github.com/johnwilander))
  * [HTTPStateTokens](https://github.com/mikewest/http-state-tokens) / Cookies
* 14:30 - 15:30 - Feature Controls
  * [Feature/Document/* Policy](https://www.w3.org/TR/feature-policy/) ([@clelland](https://github.com/clelland))
    * [Cookie Controls](https://github.com/w3c/webappsec-feature-policy/issues/85)
  * Protecting/sandboxing `<iframe>` sites (history.length, caches, window[i])
  * [Origin Policy](https://wicg.github.io/origin-policy/)
* 15:30 - 16:00 - ☕ Coffee ☕
* 16:00 - 17:00 - Injection
  * [Trusted Types](https://github.com/WICG/trusted-types)
  * [CSP3](https://github.com/w3c/webappsec-csp)
  * [CSP Next](https://github.com/mikewest/csp-next)

---

## Topics

* Old Things
    * For the third year in a row, how do we get [Referrer Policy](https://www.w3.org/TR/referrer-policy/), [Secure Contexts](https://www.w3.org/TR/secure-contexts/), [Mixed Content](https://www.w3.org/TR/mixed-content/), and [Upgrade Insecure Requests](https://www.w3.org/TR/upgrade-insecure-requests/) to REC?
    * Ditto for [Clear-Site-Data](https://www.w3.org/TR/clear-site-data/), [Credential Management](https://www.w3.org/TR/credential-management/).
    * What are we doing with [Content Security Policy](https://www.w3.org/TR/csp/) and [Embedded Enforcement](https://www.w3.org/TR/csp-embedded-enforcement/)
    * ...
* Less-old Things
    * [Fetch Metadata](https://www.w3.org/TR/fetch-metadata/)
    * [Origin Policy](https://wicg.github.io/origin-policy/)
    * [CORS-RFC1918](https://wicg.github.io/cors-rfc1918/)
    * [Feature/Document/* Policy](https://www.w3.org/TR/feature-policy/) (@clelland?)
        * [Cookie Controls](https://github.com/w3c/webappsec-feature-policy/issues/85)
    * CORP/COEP/COOP + 👻 Spectre 👻
    * ...
* New Things
    * [Trusted Types](https://github.com/WICG/trusted-types) update. Adopt into the WG? ([@koto](https://github.com/koto))
    * HTTP State Tokens
    * Mixed Content 2 ([@estark37](https://github.com/estark37))
    * [`IsLoggedIn` API](https://lists.w3.org/Archives/Public/public-webappsec/2019Sep/0004.html) ([@johnwilander](https://github.com/johnwilander))
    * [CSP Next?](https://github.com/mikewest/csp-next)
    * Double-keyed (or more) caches
    * Protecting/sandboxing <iframe> sites (history.length, caches, window[i])
    * `Sec-Origin` (@deian)
    * ...
* Process Things
    * [Charter](https://www.w3.org/2019/03/webappsec-2019-charter.html) still reasonable?
        * Putting privacy more clearly in scope and make browser privacy policies part of the security review process
    * [Evergreen standards](https://www.w3.org/wiki/Evergreen_Standards)?
    * Relationship with other groups (TAG, PING, HTTPbis, etc.)
    * Security reviews of upcoming features.
    * Various browsers' launch processes
    
Suggestions? https://github.com/w3c/webappsec/issues/555 would be a great place to make them.