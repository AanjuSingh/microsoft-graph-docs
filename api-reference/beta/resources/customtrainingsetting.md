---
title: "customTrainingSetting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# customTrainingSetting resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [trainingSetting](../resources/trainingsetting.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|dueDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [trainingSetting](../resources/trainingsetting.md).|
|dueDays|Int32|**TODO: Add Description** Inherited from [trainingSetting](../resources/trainingsetting.md).|
|durationInMinutes|String|**TODO: Add Description**|
|settingType|trainingSettingType|**TODO: Add Description** Inherited from [trainingSetting](../resources/trainingsetting.md).The possible values are: `none`, `microsoft`, `noTraining`, `custom`, `unknownFutureValue`.|
|url|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|training|[training](../resources/training.md)|**TODO: Add Description** Inherited from [microsoft.graph.trainingSetting](../resources/trainingsetting.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customTrainingSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customTrainingSetting",
  "dueDays": "Integer",
  "dueDateTime": "String (timestamp)",
  "settingType": "String",
  "url": "String",
  "displayName": "String",
  "description": "String",
  "durationInMinutes": "String"
}
```

