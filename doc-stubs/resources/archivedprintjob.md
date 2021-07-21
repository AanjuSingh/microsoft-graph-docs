---
title: "archivedPrintJob resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# archivedPrintJob resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acquiredByPrinter|Boolean|**TODO: Add Description**|
|acquiredDateTime|DateTimeOffset|**TODO: Add Description**|
|blackAndWhitePageCount|Int32|**TODO: Add Description**|
|colorPageCount|Int32|**TODO: Add Description**|
|completionDateTime|DateTimeOffset|**TODO: Add Description**|
|copiesPrinted|Int32|**TODO: Add Description**|
|createdBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|duplexPageCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|pageCount|Int32|**TODO: Add Description**|
|printerId|String|**TODO: Add Description**|
|processingState|printJobProcessingState|**TODO: Add Description**. Possible values are: `unknown`, `pending`, `processing`, `paused`, `stopped`, `completed`, `canceled`, `aborted`.|
|simplexPageCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.archivedPrintJob"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.archivedPrintJob",
  "acquiredByPrinter": "Boolean",
  "acquiredDateTime": "String (timestamp)",
  "blackAndWhitePageCount": "Integer",
  "colorPageCount": "Integer",
  "completionDateTime": "String (timestamp)",
  "copiesPrinted": "Integer",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "createdDateTime": "String (timestamp)",
  "duplexPageCount": "Integer",
  "id": "String (identifier)",
  "pageCount": "Integer",
  "printerId": "String",
  "processingState": "String",
  "simplexPageCount": "Integer"
}
```

