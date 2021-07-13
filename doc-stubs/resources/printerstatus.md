---
title: "printerStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printerStatus resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|details|printerProcessingStateDetail collection|**TODO: Add Description**|
|processingState|printerProcessingState|**TODO: Add Description**. Possible values are: `unknown`, `idle`, `processing`, `stopped`, `unknownFutureValue`.|
|processingStateDescription|String|**TODO: Add Description**|
|processingStateReasons|printerProcessingStateReason collection|**TODO: Add Description**|
|state|printerProcessingState|**TODO: Add Description**. Possible values are: `unknown`, `idle`, `processing`, `stopped`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerStatus",
  "description": "String",
  "details": [
    "String"
  ],
  "processingState": "String",
  "processingStateDescription": "String",
  "processingStateReasons": [
    "String"
  ],
  "state": "String"
}
```

