---
title: "windowsKioskActiveDirectoryGroup resource type"
description: "The class used to identify an Azure Directory group for the kiosk configuration"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsKioskActiveDirectoryGroup resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The class used to identify an Azure Directory group for the kiosk configuration


Inherits from [windowsKioskUser](../resources/windowskioskuser.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|groupName|String|The name of the AD group that will be locked to this kiosk configuration|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```

