---
title: "win32LobAppReturnCode resource type"
description: "Contains return code properties for a Win32 App"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# win32LobAppReturnCode resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains return code properties for a Win32 App

## Properties
|Property|Type|Description|
|:---|:---|:---|
|returnCode|Int32|Return code.|
|type|win32LobAppReturnCodeType|The type of return code. Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": "Integer",
  "type": "String"
}
```

