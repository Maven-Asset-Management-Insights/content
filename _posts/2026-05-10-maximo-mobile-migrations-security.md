---
layout: post
title: "Migrating Maximo Mobile Configurations Between Environments"
subtitle: "What to copy, what to skip, and how to avoid compilation errors on the other side"
date: 2026-05-10
categories:
  - insights
  - maximo
  - mobile
  - troubleshooting
tags:
  - maximo
  - mobile
  - migration
  - security
  - configuration
content_type: insight
maximo_versions:
  mas:
   - "MAS 9+"
---

Migrating Maximo Mobile application XML between environments is straightforward in concept — copy the XML from the source, paste it into the destination — but a few consistent pitfalls cause most of the compilation errors teams encounter during migrations.

## What to copy and what to skip.

The Maximo Mobile Code Editor displays the full application XML, starting with the `<maximo-application>` root element. That first line contains environment-specific attributes that should not be copied:

```xml
<maximo-application
  controller="AppController"
  default-log-level="error"
  id="YOURMOBILEAPP"
  mas-enabled="false"
  mas-id="manage"
  nav-initial-open-state="false"
  navigator-tile-order="100"
  product-name="Maximo"
  product-name-adaptive="Maximo"
  theme="touch"
  title="Technician"
  user-menu-enabled="true"
  version="9.1.22.0">
```

Attributes like `id`, `version`, `mas-id`, and `product-name` are environment-specific. Copying them into a destination environment with different values — or a different Maximo Application Suite version — can cause compilation errors that are difficult to trace.

The safer approach: copy everything below the first line. Paste the `<properties>` block and all subsequent content into the destination environment's existing root element, rather than replacing the root element itself.

## Version differences matter.

Be aware of version differences between source and destination environments. Application XML that compiles cleanly in MAS 9.1.22 may reference components or property names that don't exist in an earlier version. When migrating to a lower version, review the `<properties>` block carefully for any version-specific references.

This is also relevant in reverse: migrating from an older environment to a newer one can introduce deprecated attributes that generate warnings or errors in the new version.

## Security: two permissions to check.

Maximo Mobile security is configured in the Security Groups application under the **Options for [application]** section. Two specific options control mobile access and are easy to miss:

**Read access to Maximo mobile application** — This option grants the security group permission to access the mobile application at all. Without it, users in that group will not be able to open the mobile app even if their Maximo credentials are valid.

**Enable access to the work center with disconnected capabilities** — This option enables offline mode for the group. Without it, users will not be able to use the mobile app in areas without network connectivity — which defeats a core purpose of the mobile architecture.

Both options appear under **Actions → Grant Listed Options for This Application** in the Security Groups application. They are not enabled by default and must be explicitly granted as part of any new mobile rollout.

## The migration checklist in practice.

Before completing a mobile migration:

1. Copy only from below the root `<maximo-application>` element
2. Verify version compatibility between source and destination
3. Regenerate the mobile schema after applying XML changes: `https://<manageServer>/maximo/oslc/graphite/mobile/schema?regenerate=1`
4. Confirm security group options are set for all relevant groups
5. Test on both RBA and mobile device before signoff

[System record integrity](https://maven-asset-management-insights.github.io/content/glossary/#system-record-integrity) in mobile deployments depends on all five steps completing cleanly — a migration that skips the schema refresh or security check can produce inconsistent behavior that's hard to diagnose after the fact.

→ [Maximo Mobile 9.0: Advancing Technician Productivity](https://www.mavenasset.com/blog/maximo-mobile-9-0-advancing-technician-productivity/)
