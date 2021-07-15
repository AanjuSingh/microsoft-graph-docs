---
title: "iosAvailableUpdateVersion resource type"
description: "iOS available update version details"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# iosAvailableUpdateVersion resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

iOS available update version details

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset|The expiration date of the update.|
|postingDateTime|DateTimeOffset|The posting date of the update.|
|productVersion|String|The version of the update.|
|supportedDevices|String collection|List of supported devices for the update.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAvailableUpdateVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAvailableUpdateVersion",
  "expirationDateTime": "String (timestamp)",
  "postingDateTime": "String (timestamp)",
  "productVersion": "String",
  "supportedDevices": [
    "String"
  ]
}
```

