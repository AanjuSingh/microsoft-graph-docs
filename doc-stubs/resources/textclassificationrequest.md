---
title: "textClassificationRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# textClassificationRequest resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List textClassificationRequests](../api/textclassificationrequest-list.md)|[textClassificationRequest](../resources/textclassificationrequest.md) collection|Get a list of the [textClassificationRequest](../resources/textclassificationrequest.md) objects and their properties.|
|[Create textClassificationRequest](../api/textclassificationrequest-create.md)|[textClassificationRequest](../resources/textclassificationrequest.md)|Create a new [textClassificationRequest](../resources/textclassificationrequest.md) object.|
|[Get textClassificationRequest](../api/textclassificationrequest-get.md)|[textClassificationRequest](../resources/textclassificationrequest.md)|Read the properties and relationships of a [textClassificationRequest](../resources/textclassificationrequest.md) object.|
|[Update textClassificationRequest](../api/textclassificationrequest-update.md)|[textClassificationRequest](../resources/textclassificationrequest.md)|Update the properties of a [textClassificationRequest](../resources/textclassificationrequest.md) object.|
|[Delete textClassificationRequest](../api/textclassificationrequest-delete.md)|None|Deletes a [textClassificationRequest](../resources/textclassificationrequest.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fileExtension|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|matchTolerancesToInclude|mlClassificationMatchTolerance|**TODO: Add Description**. Possible values are: `exact`, `near`.|
|scopesToRun|sensitiveTypeScope|**TODO: Add Description**. Possible values are: `fullDocument`, `partialDocument`.|
|sensitiveTypeIds|String collection|**TODO: Add Description**|
|text|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.textClassificationRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.textClassificationRequest",
  "id": "String (identifier)",
  "fileExtension": "String",
  "matchTolerancesToInclude": "String",
  "scopesToRun": "String",
  "sensitiveTypeIds": [
    "String"
  ],
  "text": "String"
}
```

