---
title: "deviceCategory resource type"
description: "Device categories provides a way to organize your devices. Using device categories, company administrators can define their own categories that make sense to their company. These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment. You can filter reports and create dynamic Azure Active Directory device groups based on device categories."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceCategory resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device categories provides a way to organize your devices. Using device categories, company administrators can define their own categories that make sense to their company. These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment. You can filter reports and create dynamic Azure Active Directory device groups based on device categories.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceCategories](../api/devicecategory-list.md)|[deviceCategory](../resources/devicecategory.md) collection|Get a list of the [deviceCategory](../resources/devicecategory.md) objects and their properties.|
|[Create deviceCategory](../api/devicecategory-create.md)|[deviceCategory](../resources/devicecategory.md)|Create a new [deviceCategory](../resources/devicecategory.md) object.|
|[Get deviceCategory](../api/devicecategory-get.md)|[deviceCategory](../resources/devicecategory.md)|Read the properties and relationships of a [deviceCategory](../resources/devicecategory.md) object.|
|[Update deviceCategory](../api/devicecategory-update.md)|[deviceCategory](../resources/devicecategory.md)|Update the properties of a [deviceCategory](../resources/devicecategory.md) object.|
|[Delete deviceCategory](../api/devicecategory-delete.md)|None|Deletes a [deviceCategory](../resources/devicecategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Optional description for the device category.|
|displayName|String|Display name for the device category.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|roleScopeTagIds|String collection|Optional role scope tags for the device category.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

