---
title: "userFlowPageLayout resource type"
description: The amount of page layouts can be modified, only the present set of entities allows updated for "pageUri" and "version"."
author: "almars"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# userFlowPageLayout resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains details about the user flow's page layout.

Azure Active Directory B2C (Azure AD B2C) periodically releases improvements and fixes with each new page layout version. Organizations can browse available AD B2C user flow page layouts and update them to the latest versions.

> [!IMPORTANT]
> We highly recommend you keep your page layout versions up-to-date so that all page elements reflect the latest security enhancements, accessibility standards, and your feedback.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List userFlowPageLayouts](../api/userflowpagelayout-list.md)|[userFlowPageLayout](../resources/userflowpagelayout.md) collection|Get a list of the [userFlowPageLayout](../resources/userflowpagelayout.md) objects and their properties.|
|[Create userFlowPageLayout](../api/b2cidentityuserflow-post-pagelayouts.md)|[userFlowPageLayout](../resources/userflowpagelayout.md)|Create a new [userFlowPageLayout](../resources/userflowpagelayout.md) object.|
|[Get userFlowPageLayout](../api/userflowpagelayout-get.md)|[userFlowPageLayout](../resources/userflowpagelayout.md)|Read the properties and relationships of a [userFlowPageLayout](../resources/userflowpagelayout.md) object.|
|[Update userFlowPageLayout](../api/userflowpagelayout-update.md)|[userFlowPageLayout](../resources/userflowpagelayout.md)|Update the properties of a [userFlowPageLayout](../resources/userflowpagelayout.md) object.|
|[Delete userFlowPageLayout](../api/userflowpagelayout-delete.md)|None|Deletes a [userFlowPageLayout](../resources/userflowpagelayout.md) object.|
|[availableVersions](../api/userflowpagelayout-availableversions.md)|String collection|Show the supported version of page layout to provide admins and developers the exact values allowed to use.|
|[restoreDefaultPageUri](../api/userflowpagelayout-restoredefaultpageuri.md)|None|Restore the default value of the "pageUri" property.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Page name used to provide more description.|
|id|String|ID of the page layout, as used in the service.|
|isCustomPageUri|Boolean|If the page has a custom page uri, for query purpose.|
|pageUri|String|Location for the ".html" resource used to load the custom content, as show in [documentation](https://docs.microsoft.com/azure/active-directory-b2c/customize-ui-with-html?pivots=b2c-user-flow#4-update-the-user-flow).|
|version|String|Version of the page layout.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowPageLayout",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userFlowPageLayout",
  "id": "String (identifier)",
  "displayName": "String",
  "isCustomPageUri": "Boolean",
  "pageUri": "String",
  "version": "String"
}
```

