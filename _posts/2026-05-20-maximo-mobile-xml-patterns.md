---
layout: post
title: "Three XML Patterns Every Maximo Mobile Developer Should Know"
subtitle: "Hiding fields, enforcing required inputs, and locking read-only values in mobile application XML"
date: 2026-05-20
categories:
  - insights
  - maximo
  - mobile
tags:
  - maximo
  - mobile
  - xml
  - configuration
  - development
content_type: insight
maximo_versions:
  mas:
    - "MAS 8+"
    - "MAS 9+"
  maximo:
    - "7.6+"
---

Maximo Mobile application behavior is controlled through XML configuration. The Maximo Application Framework provides a set of XML patterns that cover the most common customization needs — and three of them come up on nearly every mobile project: hiding objects conditionally, making fields required, and making fields read-only.

Understanding these patterns well reduces rework. Getting them wrong in mobile is often less obvious than in the RBA, because the mobile app may simply not surface an error — it just won't behave as expected.

## Hiding objects and fields conditionally.

The most common use case is hiding a UI element based on device context — showing something in the browser that shouldn't appear on mobile, or vice versa.

```xml
<dropdown-item
  value="serverSearch"
  text="Search all records"
  hidden="{!app.device.isMaximoMobile}"
  id="serverSearchDropdown"/>
```

The `hidden` attribute accepts an expression. `{!app.device.isMaximoMobile}` evaluates to `true` when the user is on a mobile device — so this item is hidden on mobile and visible in the browser. Reversing the logic (`{app.device.isMaximoMobile}`) hides it in the browser and shows it on mobile.

This is also the pattern to check when a configuration works in RBA but doesn't appear in mobile. A hidden tag on an element is easy to miss and can look like a data or Object Structure problem when it isn't.

## Making fields required.

Required field validation in mobile is set directly in the XML using the `required` attribute:

```xml
<text-input id="description" label="Description" required="true" />
<number-input id="quantity" label="Quantity" required="true" />
```

Setting `required="true"` prevents [work order closeout](https://maven-asset-management-insights.github.io/content/glossary/#work-order-closeout) or form submission until the field is populated. This is one of the most direct ways to enforce [closeout quality](https://maven-asset-management-insights.github.io/content/glossary/#closeout-quality) and [work order data quality](https://maven-asset-management-insights.github.io/content/glossary/#work-order-data-quality) standards in the field — the application itself becomes the enforcement mechanism rather than relying on technician discipline alone.

## Making fields read-only.

Some fields should be visible on mobile for reference but should not be editable. The `readonly` attribute handles this:

```xml
<text-input
  id="wonum"
  label="Work Order"
  value="{item.wonum}"
  readonly="true" />
```

Read-only fields are particularly useful for displaying reference data — like the [work order](https://maven-asset-management-insights.github.io/content/glossary/#work-order-wo) number, asset information, or location — that technicians need to see but should not be able to change in the field.

## Customizing mobile queries.

Beyond field-level configuration, mobile queries themselves can be overridden through the `maximo-datasource-override` element. This controls what [work orders](https://maven-asset-management-insights.github.io/content/glossary/#work-order-wo) are pulled into the mobile list view:

```xml
<maximo-datasource-override
  id="myworkDS"
  mobile-qbe-filter="{{'status_maxvalue': '!=COMP,CAN,CLOSE,WAPPR'}}"
  offline-immediate-download="false"
  saved-query="MYWORK"/>
```

The `saved-query` attribute references a named query defined in the Object Structure's Query Definition. Modifying the query clause there — rather than in the application XML — controls what data the mobile database pulls down. In the example above, the MYWORK query filters out completed, cancelled, closed, and waiting-for-approval work orders from the technician's list view.

These four patterns — conditional hiding, required fields, read-only fields, and query overrides — cover the majority of mobile [work management consistency](https://maven-asset-management-insights.github.io/content/glossary/#work-management-consistency) customizations encountered in the field.
