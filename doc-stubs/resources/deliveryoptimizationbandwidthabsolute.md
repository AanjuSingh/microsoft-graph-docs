---
title: "deliveryOptimizationBandwidthAbsolute resource type"
description: "Bandwidth limits in kilobytes per second."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deliveryOptimizationBandwidthAbsolute resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Bandwidth limits in kilobytes per second.


Inherits from [deliveryOptimizationBandwidth](../resources/deliveryoptimizationbandwidth.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|maximumDownloadBandwidthInKilobytesPerSecond|Int64|Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization. Valid values 0 to 4294967295
The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads. Valid values 0 to 4294967295|
|maximumUploadBandwidthInKilobytesPerSecond|Int64|Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000). Valid values 0 to 4000000
The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth). Valid values 0 to 4000000|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": "Integer",
  "maximumUploadBandwidthInKilobytesPerSecond": "Integer"
}
```

