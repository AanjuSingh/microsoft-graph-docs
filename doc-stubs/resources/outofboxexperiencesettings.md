---
title: "outOfBoxExperienceSettings resource type"
description: "Out of box experience setting"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# outOfBoxExperienceSettings resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Out of box experience setting

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceUsageType|windowsDeviceUsageType|AAD join authentication type. Possible values are: `singleUser`, `shared`.|
|hideEscapeLink|Boolean|If set to true, then the user can't start over with different account, on company sign-in|
|hideEULA|Boolean|Show or hide EULA to user|
|hidePrivacySettings|Boolean|Show or hide privacy settings to user|
|skipKeyboardSelectionPage|Boolean|If set, then skip the keyboard selection page if Language and Region are set|
|userType|windowsUserType|Type of user. Possible values are: `administrator`, `standard`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "deviceUsageType": "String",
  "hideEscapeLink": "Boolean",
  "hideEULA": "Boolean",
  "hidePrivacySettings": "Boolean",
  "skipKeyboardSelectionPage": "Boolean",
  "userType": "String"
}
```

