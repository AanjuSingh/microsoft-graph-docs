---
title: "companyPortalBlockedAction resource type"
description: "Blocked actions on the company portal as per platform and device ownership types"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# companyPortalBlockedAction resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Blocked actions on the company portal as per platform and device ownership types

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|companyPortalAction|Device Action. Possible values are: `unknown`, `remove`, `reset`.|
|ownerType|ownerType|Device ownership type. Possible values are: `unknown`, `company`, `personal`.|
|platform|devicePlatformType|Device OS/Platform. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`, `androidAOSP`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyPortalBlockedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyPortalBlockedAction",
  "action": "String",
  "ownerType": "String",
  "platform": "String"
}
```

