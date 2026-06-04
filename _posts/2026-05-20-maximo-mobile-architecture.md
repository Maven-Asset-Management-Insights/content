---
layout: post
title: "Maximo Mobile Works Differently Than You Might Expect"
subtitle: "Understanding the local database architecture behind Maximo Mobile"
date: 2026-05-20
categories:
  - insights
  - maximo
  - mobile
tags:
  - maximo
  - mobile
  - architecture
  - offline
content_type: insight
maximo_versions:
  mas:
    - "MAS 8+"
    - "MAS 9+"
  maximo:
    - "7.6+"
---

Most people assume Maximo Mobile works the same way as the browser-based application — querying the Maximo database directly and displaying results in real time. It doesn't. The architecture is fundamentally different, and understanding that difference is essential before you start configuring or customizing anything.

## Maximo Mobile runs against a local database on the device.

When a technician opens the Maximo Mobile app, they are not querying the Maximo server directly. Instead, the app reads from a local [mobile database](https://maven-asset-management-insights.github.io/content/glossary/#work-order-wo) built on the device. That local database syncs back to Maximo when the device has internet connectivity — which means field teams can continue working in areas with limited or no network access.

This is the core design principle behind Maximo Mobile: it is built for disconnected environments. The local database is what makes offline [work order](https://maven-asset-management-insights.github.io/content/glossary/#work-order-wo) execution, [inspection form](https://maven-asset-management-insights.github.io/content/glossary/#inspection-form) completion, and asset lookup possible when connectivity isn't guaranteed.

## The local database is built through Maximo Object Structures.

The mobile device doesn't download everything — it builds its local database through API calls to Maximo's Object Structures. The Object Structures used by Maximo Mobile typically carry an **MXAPI** prefix, which is how you can identify them in the Object Structures application.

These structures define exactly what data gets pulled down to the device. If a field or relationship isn't included in the relevant Object Structure, the mobile app simply won't have access to it — regardless of what's configured in the application XML.

This has a practical implication: if your mobile app isn't showing data you expect, the Object Structure is often the first place to investigate, not the application configuration.

## What this means for configuration work.

Because the mobile app reads from a local database rather than querying Maximo directly, several things work differently than they do in the browser-based [Maximo Application Suite](https://maven-asset-management-insights.github.io/content/glossary/#maximo-application-suite-mas):

- Relationships available in the RBA (browser) application may not exist in the mobile database
- [Data quality](https://maven-asset-management-insights.github.io/content/glossary/#data-quality) and completeness depend on what the Object Structure is pulling down
- Schema changes require a mobile database refresh — not just an application save
- Testing configurations in the browser does not confirm they will behave the same way on mobile

The mobile schema can be regenerated using the following URL pattern:

```
https://<manageServer>/maximo/oslc/graphite/mobile/schema?regenerate=1
```

This is a critical step when troubleshooting mobile behavior after configuration changes — especially if the mobile app appears out of sync with what has been configured.
