---
title: "propertyRule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# propertyRule resource type

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|operation|ruleOperation|**TODO: Add Description**. Possible values are: `null`, `equals`, `notEquals`, `contains`, `notContains`, `lessThan`, `greaterThan`, `startsWith`, `unknownFutureValue`.|
|property|String|**TODO: Add Description**|
|values|String collection|**TODO: Add Description**|
|valuesJoinedBy|binaryOperator|**TODO: Add Description**. Possible values are: `or`, `and`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.propertyRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalConnectors.propertyRule",
  "property": "String",
  "operation": "String",
  "valuesJoinedBy": "String",
  "values": [
    "String"
  ]
}
```

