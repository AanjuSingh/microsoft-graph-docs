---
title: "scheduleChangeRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# scheduleChangeRequest resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**
This is an abstract type.


Inherits from [changeTrackedEntity](../resources/changetrackedentity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List scheduleChangeRequests](../api/schedulechangerequest-list.md)|[scheduleChangeRequest](../resources/schedulechangerequest.md) collection|Get a list of the [scheduleChangeRequest](../resources/schedulechangerequest.md) objects and their properties.|
|[Create scheduleChangeRequest](../api/schedulechangerequest-create.md)|[scheduleChangeRequest](../resources/schedulechangerequest.md)|Create a new [scheduleChangeRequest](../resources/schedulechangerequest.md) object.|
|[Get scheduleChangeRequest](../api/schedulechangerequest-get.md)|[scheduleChangeRequest](../resources/schedulechangerequest.md)|Read the properties and relationships of a [scheduleChangeRequest](../resources/schedulechangerequest.md) object.|
|[Update scheduleChangeRequest](../api/schedulechangerequest-update.md)|[scheduleChangeRequest](../resources/schedulechangerequest.md)|Update the properties of a [scheduleChangeRequest](../resources/schedulechangerequest.md) object.|
|[Delete scheduleChangeRequest](../api/schedulechangerequest-delete.md)|None|Deletes a [scheduleChangeRequest](../resources/schedulechangerequest.md) object.|
|[approve](../api/schedulechangerequest-approve.md)|None|**TODO: Add Description**|
|[decline](../api/schedulechangerequest-decline.md)|None|**TODO: Add Description**|
|[stageForDeletion](../api/schedulechangerequest-stagefordeletion.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedTo|scheduleChangeRequestActor|**TODO: Add Description**. The possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md).|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md).|
|id|String|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md).|
|managerActionDateTime|DateTimeOffset|**TODO: Add Description**|
|managerActionMessage|String|**TODO: Add Description**|
|managerUserId|String|**TODO: Add Description**|
|senderDateTime|DateTimeOffset|**TODO: Add Description**|
|senderMessage|String|**TODO: Add Description**|
|senderUserId|String|**TODO: Add Description**|
|state|scheduleChangeState|**TODO: Add Description**. The possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.scheduleChangeRequest",
  "baseType": "Microsoft.Teams.Shifts.changeTrackedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scheduleChangeRequest",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "String",
  "senderDateTime": "String (timestamp)",
  "managerActionMessage": "String",
  "managerActionDateTime": "String (timestamp)",
  "senderUserId": "String",
  "managerUserId": "String"
}
```

