---
title: "deviceEnrollmentPlatformRestriction resource type"
description: "Platform specific enrollment restrictions"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceEnrollmentPlatformRestriction resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Platform specific enrollment restrictions

## Properties
|Property|Type|Description|
|:---|:---|:---|
|blockedManufacturers|String collection|Collection of blocked Manufacturers.|
|blockedSkus|String collection|Collection of blocked Skus.|
|osMaximumVersion|String|Max OS version supported|
|osMinimumVersion|String|Min OS version supported|
|personalDeviceEnrollmentBlocked|Boolean|Block personally owned devices from enrolling|
|platformBlocked|Boolean|Block the platform from enrolling|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "blockedManufacturers": [
    "String"
  ],
  "blockedSkus": [
    "String"
  ],
  "osMaximumVersion": "String",
  "osMinimumVersion": "String",
  "personalDeviceEnrollmentBlocked": "Boolean",
  "platformBlocked": "Boolean"
}
```

