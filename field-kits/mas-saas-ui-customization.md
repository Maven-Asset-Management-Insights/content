---
layout: default
title: "MAS SaaS: Unlock Suite Administration and Brand Your Interface"
description: "IBM now allows MAS SaaS administrators to manage Suite Configurations, Authentication, and User Sessions, but the access isn't granted automatically. Here's how to request it and customize your header."
permalink: /field-kits/mas-saas-ui-customization/
---

# MAS SaaS: Unlock Suite Administration and Brand Your Interface

*Contributed by Randi Wagner, Senior Consultant, Maven Asset Management*

If your organization runs Maximo Application Suite (MAS) as an IBM SaaS customer, your administrators may be missing tools they are now allowed to use.

IBM previously blocked SaaS customers from several Suite Administration applications. That has changed. Administrators can now manage identity provider (IdP) settings, API keys, and user interface customization.

There's a catch. IBM rolled this out quietly and did not grant the new security to existing SaaS clients. Most customers don't know they are missing it. You have to ask.

---

## What You Get

Once access is granted, your local MAXADMIN account can use:

- **Suite > Configurations** (including User interface customization)
- **Suite > Authentication**
- **Suite > User Sessions**

Most SaaS administrators today only see:

- Suite > Catalog
- Suite > Usage

> **Note:** Once your local MAXADMIN account has these privileges, it can enable them for your other administrator accounts.

---

## Step 1: Log a Case with IBM

Open a support case with IBM requesting that your local MAXADMIN account be granted privileges for IdP and API key management. You can copy and paste the text below into your case.

```
Our URLs are:
<insert your environment URL>
<insert your dev/test environment URL> (optional)

Our local MaxAdmin account appears to be missing Suite Administration
privileges including:

Suite > Configurations (including User interface customization)
Suite > Authentication
Suite > User Sessions

The only options we have are:
Suite > Catalog
Suite > Usage

Please grant these rights to the following user in all environments.
MAXADMIN

The security is specifically needed to modify CSS
(https://www.ibm.com/support/pages/override-maximo-application-suite-header-color-using-css-customization-mas-admin-dashboard)
```

> **Best Practice:** List every environment you want covered (production and dev/test) so you only need to log one case.

---

## Step 2: Open the Configurations Application

Navigate to:

**Suite Administration > Configurations**

> **Note:** This application sometimes takes a few seconds to fully load.

From here you can see your current SAML and SMTP configurations, along with options to customize the user interface. Select **User interface customization**.

![MAS Suite Administration Configurations page with User interface customization highlighted]({{ 'assets/img/01-configurations-app.png' | relative_url }})

---

## Step 3: Change the Company and Product Name

Navigate to:

**Suite Administration > Configurations > User interface customization > Header configuration**

This tab controls the company name and product name shown in the upper left corner of the header. By default, these read "IBM" and "Maximo Application Suite."

![Header configuration tab showing the default IBM company name and Maximo Application Suite product name]({{ '/assets/img/field-kits/mas-saas-ui-customization/02-header-config-default.png' | relative_url }})

### Steps

1. Enter your organization's name in **Company name**
2. Enter a label in **Product name** (an environment name works well here)
3. Optionally, upload a logo to appear before the company name
4. Save your changes

> **Note:** Logos must be .svg or .png files, 1 MB or smaller. The optimum height is 40 pixels or less. To remove a logo, delete the file.

Here's the result in Maven's demo environment, with the header now reading "Maven Asset Management MVNDEMO02":

![Header configuration with Maven Asset Management as the company name and MVNDEMO02 as the product name]({{ '/assets/img/field-kits/mas-saas-ui-customization/03-header-config-branded.png' | relative_url }})

> **Best Practice:** Use the product name to show which environment users are in (for example, PROD, TEST, or DEV). It's a simple way to keep people from making changes in the wrong system.

---

## Step 4: Change the Header Color with CSS

Navigate to:

**Suite Administration > Configurations > User interface customization > CSS customization**

### Steps

1. Turn on **Enable CSS customization**
2. Add your CSS in the editor
3. Click **Save and publish** to apply the change globally

### Example: Change the Header to Blue

```css
/*Header Background Color */
.cds--header{
  background-color: royalblue
}
```

![CSS customization tab with the header background set to royal blue]({{ '/assets/img/field-kits/mas-saas-ui-customization/04-css-header-color.png' | relative_url }})

> **Warning:** Some CSS classes are shared across multiple applications, which can cause unexpected results. Classes may also change or be removed when you upgrade. To return to the default styling, turn **Enable CSS customization** off.

> **Best Practice:** Pair a header color with each environment. When production is one color and test is another, users can tell at a glance where they are.

---

## Resources

- IBM documentation: [Updating the user interface](https://www.ibm.com/docs/en/masv-and-l/cd?topic=interface-updating-user)
- IBM support: [Override the MAS header color using CSS customization](https://www.ibm.com/support/pages/override-maximo-application-suite-header-color-using-css-customization-mas-admin-dashboard)

---

A few minutes with an IBM case and the Configurations app gives your administrators control they are already entitled to. Need help with MAS administration or configuration? [Email Maven](mailto:mas@mavenasset.com).
