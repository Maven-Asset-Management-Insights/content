---
layout: post
title: "RBA and Mobile Are Not the Same Application. Treat Them That Way."
subtitle: "Why configurations that work in the browser may silently fail on mobile"
date: 2026-05-20
categories:
  - insights
  - maximo
  - mobile
  - troubleshooting
tags:
  - maximo
  - mobile
  - rba
  - troubleshooting
  - configuration
content_type: insight
maximo_versions:
  mas:
    - "MAS 8+"
    - "MAS 9+"
  maximo:
    - "7.6+"
---

One of the most common sources of confusion when customizing Maximo Mobile is the assumption that the browser-based application (RBA) and the mobile application behave the same way. They look similar. They share configuration concepts. But they run on fundamentally different data sources — and that difference has real consequences for development and testing.

## The core difference: where data comes from.

The RBA application queries the Maximo database directly. It has access to the full object model, all relationships, and any data that exists in the system at the time of the query.

The Maximo Mobile application does not query the Maximo database directly. It queries the local database built on the device — a subset of Maximo data defined by the [Mobile Object Structures](https://maven-asset-management-insights.github.io/content/glossary/#mobile-object-structures) that populated it. If a relationship or field wasn't pulled into the local database, mobile simply doesn't have it, even if RBA works perfectly.

This means:

- A query that returns results in RBA may return nothing in mobile
- A field that displays correctly in the browser may not appear on the device
- A configuration that works in the browser environment may not exist in the mobile application at all

Out of the box, certain fields and queries are visible on mobile that are not present in RBA, and vice versa. Neither is wrong — they are different applications with different data scopes.

## A real example: the hidden query problem.

During development work on the TECHMOBILE application, configurations were completed and verified in RBA — and then failed to appear in mobile. The root cause: a conditional tag in the application XML was hiding the functionality on mobile. The configuration was correct, but a visibility condition was suppressing it based on the device context.

The fix: check whether a tag is conditionally hiding the element using `{!app.device.isMaximoMobile}` or similar device-context expressions before assuming the configuration is wrong.

## Always test both.

The practical rule: **never assume RBA behavior reflects mobile behavior.** When doing development work on mobile applications, test both the RBA and mobile versions after every significant change. Issues that only appear on one surface are easy to miss — and can result in a configuration that passes review but fails in the field.

The schema refresh URL is also worth keeping handy during testing:

```
https://<manageServer>/maximo/oslc/graphite/mobile/schema?regenerate=1
```

If mobile behavior doesn't reflect your latest changes, regenerating the schema is often the first step — not a reconfiguration of the application XML.

→ [Maximo Mobile 9.0: Advancing Technician Productivity](https://www.mavenasset.com/blog/maximo-mobile-9-0-advancing-technician-productivity/)
