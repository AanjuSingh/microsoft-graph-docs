---
title: "Use the employee learning API to integrate with Viva Learning"
description: "Learn how to register a provider, and integrate your content and learner records from your learning provider to Viva Learning."
ms.localizationpriority: medium
author: "malabikaroy"
ms.prod: "employee-learning"
doc_type: conceptualPageType
---

# Use the employee learning API to integrate with Viva Learning

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Viva Learning is a centralized employee learning hub in Microsoft Teams that lets employees integrate learning and building skills into their work day. In Viva Learning, teams can discover, share, recommend, and learn from content libraries provided by both their organization and partners. They can quickly access assigned or recently completed learning content, and do all of this without leaving Microsoft Teams.

The employee learning API in Microsoft Graph enable apps to make content from a Learning Management System (LMS) or learning provider available in Viva Learning. Use the following resources to integrate with Viva Learning:

- Learning provider to manage learning providers, including registering, enabling, disabling, or deleting providers.
- Learning content to upload and manage learning content metadata from your LMS or learning provider in Viva Learning.


## How integrations work?
As administrators, you can integrate your content and learner records (employee assignments and completed course records) from your Learning Management System (LMS) or learning provider with Viva Learning, by using out-of-the-box integrations where Viva Learning can pull content metadata and learning records from your LMS or learning provider. You can also [use the employee learning API](#use-cases-of-the-employee-learning-api-in-microsoft-graph) in Microsoft Graph to push content metadata from your LMS or learning provider into Viva Learning. 

Once the content metadata, employee assignments, and their completed course records are uploaded to Viva Learning, they appear in Viva Learning at the following locations:
- The content appears on the home page under the **Browse courses** – **Providers** section.
- Assignments and completed course records appear on the **My Learning** page under the **Assigned to you** and **Completed** sections respectively.

## Authorization
With the appropriate delegated or application [employee learning permissions](/graph/permissions-reference#employee-learning-permissions), your app can use the employee learning API to manage learning providers and their content for a learning hub in a tenant. For more information on access tokens, app registration, and delegated and application permissions, see [Authentication and authorization basics](/graph/auth/auth-concepts).

## Use cases of the employee learning API in Microsoft Graph
Use the employee learning APIs to do the following:
- Register a provider with Viva Learning, provide a display name, square logo that is displayed on a learning content card, and a long logo that is displayed in the *Details* page which is required for the provider content to show up in Viva Learning. The returned registration ID can be used to make the subsequent calls for content ingestion.
- Enable or disable a registration and update the display name  and logo URLs  for a provider.  
- Retrieve the details about a provider in Viva Learning for a specific **registrationId**.  
- Retrieve the list of registrations in Viva Learning for the provider using the Microsoft Graph API.
- Delete a registration.
- Push content meta data to Viva Learning to make content available within Viva Learning for consumption by users.  
- Read the ingested content by using the **registrationId** of a provider.  
- Retrieve the properties of a learning content object.
- Delete the ingested content.

**Note**: Assignments and completed course records are not yet available in the employee learning API.

## What's new
Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.

## Next steps
- Enable employee learning using the collaborative capabilities in Teams
- Try the employee learning API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).