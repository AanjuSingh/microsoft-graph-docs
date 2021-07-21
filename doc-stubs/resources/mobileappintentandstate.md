---
title: "mobileAppIntentAndState resource type"
description: "MobileApp Intent and Install State for a given device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileAppIntentAndState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

MobileApp Intent and Install State for a given device.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List mobileAppIntentAndStates](../api/mobileappintentandstate-list.md)|[mobileAppIntentAndState](../resources/mobileappintentandstate.md) collection|Get a list of the [mobileAppIntentAndState](../resources/mobileappintentandstate.md) objects and their properties.|
|[Create mobileAppIntentAndState](../api/mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/mobileappintentandstate.md)|Create a new [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object.|
|[Get mobileAppIntentAndState](../api/mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/mobileappintentandstate.md)|Read the properties and relationships of a [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object.|
|[Update mobileAppIntentAndState](../api/mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/mobileappintentandstate.md)|Update the properties of a [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object.|
|[Delete mobileAppIntentAndState](../api/mobileappintentandstate-delete.md)|None|Deletes a [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|managedDeviceIdentifier|String|Device identifier created or collected by Intune.|
|mobileAppList|[mobileAppIntentAndStateDetail](../resources/mobileappintentandstatedetail.md) collection|The list of payload intents and states for the tenant.|
|userId|String|Identifier for the user that tried to enroll the device.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppIntentAndState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "String (identifier)",
  "managedDeviceIdentifier": "String",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
    }
  ],
  "userId": "String"
}
```

