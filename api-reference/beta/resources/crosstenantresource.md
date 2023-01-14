---
title: "crossTenantResource resource type"
description: "Contains information about the original object in the source Azure AD tenant the object was synchronized from."
author: "rolyon"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# crossTenantResource resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains information about the original object in the source Azure AD tenant the object was synchronized from. This information is only populated for objects that are synchronized using Azure AD cross-tenant synchronization.

This is an abstract type that's inherited by the [crossTenantSynchronizationResource](crosstenantsynchronizationresource.md) resource type.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|originId|String|ID of the original object in the source Azure AD tenant the object was synchronized from.|
|originTenantId|String|ID of the source Azure AD tenant.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.crossTenantResource",
  "originId": "String",
  "originTenantId": "String"
}
```

