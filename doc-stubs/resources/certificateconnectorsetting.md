---
title: "certificateConnectorSetting resource type"
description: "Certificate connector settings."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# certificateConnectorSetting resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Certificate connector settings.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certExpiryTime|DateTimeOffset|Certificate expire time|
|connectorVersion|String|Version of certificate connector|
|enrollmentError|String|Certificate connector enrollment error|
|lastConnectorConnectionTime|DateTimeOffset|Last time certificate connector connected|
|lastUploadVersion|Int64|Version of last uploaded certificate connector|
|status|Int32|Certificate connector status|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "certExpiryTime": "String (timestamp)",
  "connectorVersion": "String",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "lastUploadVersion": "Integer",
  "status": "Integer"
}
```

