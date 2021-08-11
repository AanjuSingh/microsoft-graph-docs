---
title: "deviceHealthScriptStringParameter resource type"
description: "Properties of the  String script parameter."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScriptStringParameter resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Properties of the  String script parameter.


Inherits from [deviceHealthScriptParameter](../resources/devicehealthscriptparameter.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applyDefaultValueWhenNotAssigned|Boolean|Whether Apply DefaultValue When Not Assigned Inherited from [deviceHealthScriptParameter](../resources/devicehealthscriptparameter.md).|
|defaultValue|String|The default value of string param|
|description|String|The description of the param Inherited from [deviceHealthScriptParameter](../resources/devicehealthscriptparameter.md).|
|isRequired|Boolean|Whether the param is required Inherited from [deviceHealthScriptParameter](../resources/devicehealthscriptparameter.md).|
|name|String|The name of the param Inherited from [deviceHealthScriptParameter](../resources/devicehealthscriptparameter.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptStringParameter",
  "name": "String",
  "description": "String",
  "isRequired": "Boolean",
  "applyDefaultValueWhenNotAssigned": "Boolean",
  "defaultValue": "String"
}
```

