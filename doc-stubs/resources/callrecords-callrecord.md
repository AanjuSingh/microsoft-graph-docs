---
title: "callRecord resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# callRecord resource type

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/callrecords-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List callRecords](../api/callrecords-callrecord-list.md)|[microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md) collection|Get a list of the [callRecord](../resources/callrecords-callrecord.md) objects and their properties.|
|[Create callRecord](../api/callrecords-callrecord-create.md)|[microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md)|Create a new [callRecord](../resources/callrecords-callrecord.md) object.|
|[Get callRecord](../api/callrecords-callrecord-get.md)|[microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md)|Read the properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.|
|[Update callRecord](../api/callrecords-callrecord-update.md)|[microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md)|Update the properties of a [callRecord](../resources/callrecords-callrecord.md) object.|
|[Delete callRecord](../api/callrecords-callrecord-delete.md)|None|Deletes a [callRecord](../resources/callrecords-callrecord.md) object.|
|[getDirectRoutingCalls](../api/callrecords-callrecord-getdirectroutingcalls.md)|[microsoft.graph.callRecords.directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) collection|**TODO: Add Description**|
|[getPstnCalls](../api/callrecords-callrecord-getpstncalls.md)|[microsoft.graph.callRecords.pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) collection|**TODO: Add Description**|
|[List sessions](../api/callrecords-callrecord-list-sessions.md)|[microsoft.graph.callRecords.session](../resources/callrecords-session.md) collection|Get the session resources from the sessions navigation property.|
|[Create session](../api/callrecords-callrecord-post-sessions.md)|[microsoft.graph.callRecords.session](../resources/callrecords-session.md)|Create a new session object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/callrecords-entity.md).|
|joinWebUrl|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|modalities|modality collection|**TODO: Add Description**|
|organizer|[microsoft.graph.identitySet](../resources/callrecords-identityset.md)|**TODO: Add Description**|
|participants|[microsoft.graph.identitySet](../resources/callrecords-identityset.md) collection|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|type|callType|**TODO: Add Description**. Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|version|Int64|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sessions|[microsoft.graph.callRecords.session](../resources/callrecords-session.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.callRecords.callRecord",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.callRecord",
  "id": "String (identifier)",
  "endDateTime": "String (timestamp)",
  "joinWebUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "modalities": [
    "String"
  ],
  "organizer": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "participants": [
    {
      "@odata.type": "microsoft.graph.identitySet"
    }
  ],
  "startDateTime": "String (timestamp)",
  "type": "String",
  "version": "Integer"
}
```

