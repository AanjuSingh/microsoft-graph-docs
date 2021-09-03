---
title: "permission resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# permission resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List permissions](../api/permission-list.md)|[permission](../resources/permission.md) collection|Get a list of the [permission](../resources/permission.md) objects and their properties.|
|[Create permission](../api/permission-create.md)|[permission](../resources/permission.md)|Create a new [permission](../resources/permission.md) object.|
|[Get permission](../api/permission-get.md)|[permission](../resources/permission.md)|Read the properties and relationships of a [permission](../resources/permission.md) object.|
|[Update permission](../api/permission-update.md)|[permission](../resources/permission.md)|Update the properties of a [permission](../resources/permission.md) object.|
|[Delete permission](../api/permission-delete.md)|None|Deletes a [permission](../resources/permission.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|grantedTo|[identitySet](../resources/intune-identityset.md)|**TODO: Add Description**|
|grantedToIdentities|[identitySet](../resources/intune-identityset.md) collection|**TODO: Add Description**|
|grantedToIdentitiesV2|[sharePointIdentitySet](../resources/sharepointidentityset.md) collection|**TODO: Add Description**|
|grantedToV2|[sharePointIdentitySet](../resources/sharepointidentityset.md)|**TODO: Add Description**|
|hasPassword|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|inheritedFrom|[itemReference](../resources/itemreference.md)|**TODO: Add Description**|
|invitation|[sharingInvitation](../resources/sharinginvitation.md)|**TODO: Add Description**|
|link|[sharingLink](../resources/sharinglink.md)|**TODO: Add Description**|
|roles|String collection|**TODO: Add Description**|
|shareId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permission",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.permission",
  "id": "String (identifier)",
  "expirationDateTime": "String (timestamp)",
  "grantedTo": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "grantedToIdentities": [
    {
      "@odata.type": "microsoft.graph.identitySet"
    }
  ],
  "grantedToV2": {
    "@odata.type": "microsoft.graph.sharePointIdentitySet"
  },
  "grantedToIdentitiesV2": [
    {
      "@odata.type": "microsoft.graph.sharePointIdentitySet"
    }
  ],
  "hasPassword": "Boolean",
  "inheritedFrom": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "invitation": {
    "@odata.type": "microsoft.graph.sharingInvitation"
  },
  "link": {
    "@odata.type": "microsoft.graph.sharingLink"
  },
  "roles": [
    "String"
  ],
  "shareId": "String"
}
```

