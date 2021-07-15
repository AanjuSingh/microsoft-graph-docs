---
title: "directRoutingLogRow resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# directRoutingLogRow resource type

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|calleeNumber|String|**TODO: Add Description**|
|callEndSubReason|Int32|**TODO: Add Description**|
|callerNumber|String|**TODO: Add Description**|
|callType|String|**TODO: Add Description**|
|correlationId|String|**TODO: Add Description**|
|duration|Int32|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|failureDateTime|DateTimeOffset|**TODO: Add Description**|
|finalSipCode|Int32|**TODO: Add Description**|
|finalSipCodePhrase|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|inviteDateTime|DateTimeOffset|**TODO: Add Description**|
|mediaBypassEnabled|Boolean|**TODO: Add Description**|
|mediaPathLocation|String|**TODO: Add Description**|
|signalingLocation|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|successfulCall|Boolean|**TODO: Add Description**|
|trunkFullyQualifiedDomainName|String|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.directRoutingLogRow",
  "calleeNumber": "String",
  "callEndSubReason": "Integer",
  "callerNumber": "String",
  "callType": "String",
  "correlationId": "String",
  "duration": "Integer",
  "endDateTime": "String (timestamp)",
  "failureDateTime": "String (timestamp)",
  "finalSipCode": "Integer",
  "finalSipCodePhrase": "String",
  "id": "String (identifier)",
  "inviteDateTime": "String (timestamp)",
  "mediaBypassEnabled": "Boolean",
  "mediaPathLocation": "String",
  "signalingLocation": "String",
  "startDateTime": "String (timestamp)",
  "successfulCall": "Boolean",
  "trunkFullyQualifiedDomainName": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String"
}
```

