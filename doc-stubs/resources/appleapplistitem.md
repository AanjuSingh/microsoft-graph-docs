---
title: "appleAppListItem resource type"
description: "Represents an app in the list of managed Apple applications"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appleAppListItem resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents an app in the list of managed Apple applications


Inherits from [appListItem](../resources/applistitem.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String|The application or bundle identifier of the application Inherited from [appListItem](../resources/applistitem.md).|
|appStoreUrl|String|The Store URL of the application Inherited from [appListItem](../resources/applistitem.md).|
|name|String|The application name Inherited from [appListItem](../resources/applistitem.md).|
|publisher|String|The publisher of the application Inherited from [appListItem](../resources/applistitem.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleAppListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleAppListItem",
  "appId": "String",
  "appStoreUrl": "String",
  "name": "String",
  "publisher": "String"
}
```

