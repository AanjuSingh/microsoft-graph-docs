---
title: "What's new in Microsoft Graph"
description: "What's currently new in Microsoft Graph"
author: "angelgolfer-ms"
ms.localizationpriority: high
---

# What's new in Microsoft Graph

See highlights of what's new in the recent two months in Microsoft Graph, [what's added earlier](whats-new-earlier.md), and how you can [share your ideas](#want-to-stay-in-the-loop). For a detailed list of API-level updates, see the [API changelog](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Features, including APIs and tools, in _preview_ status may change without notice, and some may never be promoted to generally available (GA) status. Do not use preview features in production apps.

## March 2022: New and generally available

### Microsoft Graph Toolkit

- Optimize refreshing of people's images in the [Person](graph/toolkit/components/person) component and use `disable-image-fetch` to control unnecessary fetching where appropriate
- Avoid unncessary loading of people's images in the [People picker](graph/toolkit/components/people-picker) component by using the `disable-images`. 
- Filter the available users, groups and list of people on the [People picker](graph/toolkit/components/people-picker) component by using the newly introduced `user-filters`, `group-filters` and `people-filters` properties.

For more information, see [v2.4.0](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases/tag/v2.4.0).


## March 2022: New in preview only


## February 2022: New and generally available

### Teamwork
Get [details about an online meeting](/graph/api/resources/teamworkOnlineMeetingInfo) that is associated with a [chat](/graph/api/resources/chat) through the **onlineMeetingInfo** property.

## February 2022: New in preview only

### Change notifications
Subscribe to changes of Outlook contacts, events, or messages to receive notifications that include resource data in the payload. For more information, see [Change notifications for Outlook resources in Microsoft Graph](outlook-change-notifications-overview.md).

### Identity and access | Directory management
Use application permissions `CustomSecAttributeAssignment.Read.All` to read [custom security attribute definitions](/graph/api/resources/customsecurityattributedefinition?view=graph-rest-beta&preserve-view=true) for an organization without a signed-in user.

### Identity and access | Governance
- Configure [settings](/graph/api/resources/accessreviewstagesettings?view=graph-rest-beta&preserve-view=true) for each [stage](/graph/api/resources/accessreviewstage?view=graph-rest-beta&preserve-view=true) in a multi-stage access review. In addition to [get](/graph/api/accessreviewstage-get?view=graph-rest-beta&preserve-view=true) or [update](/graph/api/accessreviewstage-update?view=graph-rest-beta&preserve-view=true) an access review stage, you can do the following: 
  - [Stop](/graph/api/accessreviewstage-stop?view=graph-rest-beta&preserve-view=true) reviewers from giving more input to a stage and proceed to the next stage if applicable. 
  - [Filter](/graph/api/accessreviewstage-filterbycurrentuser?view=graph-rest-beta&preserve-view=true) and get all the stages on an [access review instance](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true) for which the calling user is a reviewer
  - [List decisions](/graph/api/accessreviewstage-list-decisions?view=graph-rest-beta&preserve-view=true) from a multi-stage access review.
- Apps can use application permission `EntitlementManagement.ReadWrite.All` to [create an access package resource request](/graph/api/entitlementmanagement-post-accesspackageresourcerequests?view=graph-rest-beta&preserve-view=true) to add or remove a resource to an [access package catalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true).

### Identity and access | Identity and sign-in
- Use a number of new properties to configure an [organization's branding](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true). For example, a banner version of a company logo for the sign-in page, a custom favicon with a CDN-based URL, and a few other custom properties for users to manage accounts.
- Include or exclude Linux as one of the [platform conditions](/graph/api/resources/conditionalaccessplatforms?view=graph-rest-beta&preserve-view=true) in a [conditional access policy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Identify [at-risk service principals](/graph/api/resources/riskyserviceprincipal?view=graph-rest-beta&preserve-view=true) in an organization with Azure AD, which continually [detects and evaluates risks](/graph/api/resources/serviceprincipalriskdetection?view=graph-rest-beta&preserve-view=true) based on various signals and machine learning. You can [confirm](/graph/api/riskyserviceprincipal-confirmcompromised?view=graph-rest-beta&preserve-view=true) if an at-risk service principal is indeed compromised, upon which Microsoft would disable that service principal object. You can [dismiss](/graph/api/riskyserviceprincipal-dismiss?view=graph-rest-beta&preserve-view=true) the risk of an at-risk service principal. And, you can [list the risk history](/graph/api/riskyserviceprincipal-list-history?view=graph-rest-beta&preserve-view=true) of a service principal.
- Use [cross-tenant access settings](/graph/api/resources/crosstenantaccesspolicy-overview?view=graph-rest-beta&preserve-view=true) to control and manage collaboration between users in your organization and other organizations. They are granular to let you determine the users, groups, and apps, both in your organization and in external organizations, that can participate in Azure AD B2B collaboration and Azure AD B2B direct connect. 
- Enable or disable users and groups in an organization to use the [Azure AD native Certificate-Based Authentication (CBA)](/graph/api/resources/x509CertificateAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true).

## Want to stay in the loop?

Here are some ways we can engage:

- Are there scenarios you'd like Microsoft Graph to support? Suggest and vote for new features at [Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Some new features originate as popular requests from the developer community. The Microsoft Graph team regularly evaluates customer needs and releases new features in the following order:

    1. Debut in **_preview_** status. Any related REST API updates are in the beta endpoint (`https://graph.microsoft.com/beta`).  

    2. Promoted to **_general availability_ (GA)** status, if sufficient feedback indicates viability. Any related REST API updates are added to the v1.0 endpoint (`https://graph.microsoft.com/v1.0`). 
- Be an active member in the Microsoft Graph community! [Join](https://aka.ms/microsoftgraphcall) the monthly Microsoft Graph community call.
- Sign up for the [Microsoft 365 developer program](https://developer.microsoft.com/office/dev-program), get a free Microsoft 365 subscription, and start developing!


## See also
- Check out the [Microsoft Graph developer blog](https://developer.microsoft.com/graph/blogs/) periodically for release announcements and helpful resources.
- Browse details of Microsoft Graph API additions, and API behavior updates in the [changelog](https://developer.microsoft.com/graph/changelog/).
- Find [highlights of earlier releases](whats-new-earlier.md).
- Learn more about [versioning, support, and breaking change policies for Microsoft Graph](versioning-and-support.md).
