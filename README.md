# Simkl TV Tracker API Repository


# THESE DOCS HAVE MOVED

# New home: [api.simkl.org](https://api.simkl.org)

---

> **The Simkl developer documentation has moved to [api.simkl.org](https://api.simkl.org).**
>
> Apiary (where these docs have lived for years) is being sunset by Oracle in October 2026. All new endpoints, breaking changes, and improvements are published on the new site. The pages below are frozen as of 2026-05-22 and will be retired when Oracle pulls Apiary down.

---

## What is at the new site

The new documentation at **[api.simkl.org](https://api.simkl.org)** is a top-to-bottom rewrite, not a content port. What you will find there:

+ **Detailed workflow guides** for [Sync](https://api.simkl.org/guides/sync), [Scrobble](https://api.simkl.org/guides/scrobble), [Search](https://api.simkl.org/guides/search), [Anime](https://api.simkl.org/guides/anime), [Deep linking](https://api.simkl.org/guides/deep-linking), [Mark as watched](https://api.simkl.org/guides/mark-as-watched), and the new [Rewatches](https://api.simkl.org/guides/rewatches) guide.
+ **All three authentication flows** properly walked through at [api.simkl.org/authentication](https://api.simkl.org/authentication): OAuth 2.0 for server-side web apps, Public PKCE for mobile, SPAs, browser extensions, and desktop binaries, and the PIN flow for TVs, consoles, CLIs, and media-server plugins.
+ **Conventions pages** for the cross-cutting topics this Apiary spec never covered: [Headers](https://api.simkl.org/conventions/headers), [Pagination](https://api.simkl.org/conventions/pagination), [Dates](https://api.simkl.org/conventions/dates), [Watchlist statuses](https://api.simkl.org/conventions/list-statuses), [Null values](https://api.simkl.org/conventions/null-values), [Images](https://api.simkl.org/conventions/images), and [CORS](https://api.simkl.org/conventions/cors).
+ **A flat [Errors page](https://api.simkl.org/conventions/errors)** covering every HTTP status code, with cause, fix, and example for each.
+ **Interactive try-it-now playground** on all 48 endpoints across 14 categories. Drop in your token, hit Send, get a real response back.
+ **Copy-paste examples in 16 languages**: curl, Python, JS/TS, Kotlin, Swift, Java, Go, C#, Ruby, PowerShell, C/C++, and more.
+ **LLM-friendly**: every page can be copied as raw markdown or opened straight in Claude, ChatGPT, Cursor, or VSCode. Full-site [llms.txt](https://api.simkl.org/llms.txt) is published too.
+ **Full [OpenAPI 3.1 spec](https://api.simkl.org/openapi.json)** with every endpoint and every response shape verified against the live API. Point your SDK generator at it.

## New features shipping alongside the docs

+ **[Rewatches](https://api.simkl.org/guides/rewatches)**: `POST /sync/history?allow_rewatch=yes` now tracks separate viewing sessions on items the user already finished, the same data that powers the Rewatches panel on simkl.com. Up to 50 sessions per movie, show, or anime, with proper session IDs you can resume. Available for Simkl Pro and VIP members.
+ **[API Analytics](https://api.simkl.org/debug/api-analytics)**: every registered Simkl app now has a built-in live request log. 24 hours of individual requests, with edge and origin status codes, latency, burst detection for retry loops, and CSV export. Useful for diagnosing OAuth wrappers, sync loops missing `date_from`, and silent 4xx errors your HTTP client never surfaces. Open it from your app row in your [developer dashboard](https://simkl.com/settings/developer/).

## Where to ask questions

The Simkl team is on [Discord](https://discord.gg/MJsWNE4) and reads everything posted there. The [changelog](https://api.simkl.org/changelog) tracks every new endpoint, breaking change, and improvement.

---


[![](https://dcbadge.limes.pink/api/server/u89XfYn)](https://discord.gg/u89XfYn)

[Simkl API Documentation on Apiary](http://api.simkl.com)

by [Simkl](https://simkl.com)
