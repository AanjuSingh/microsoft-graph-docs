---
title: "win32LobAppInstallExperience resource type"
description: "Contains installation experience properties for a Win32 App"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# win32LobAppInstallExperience resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains installation experience properties for a Win32 App

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceRestartBehavior|win32LobAppRestartBehavior|Device restart behavior. Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.|
|runAsAccount|runAsAccountType|Indicates the type of execution context the app runs in. Possible values are: `system`, `user`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "deviceRestartBehavior": "String",
  "runAsAccount": "String"
}
```

