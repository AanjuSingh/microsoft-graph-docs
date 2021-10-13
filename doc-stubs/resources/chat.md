---
title: "chat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# chat resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List chats](../api/chat-list.md)|[chat](../resources/chat.md) collection|Get a list of the [chat](../resources/chat.md) objects and their properties.|
|[Create chat](../api/chat-post-chats.md)|[chat](../resources/chat.md)|Create a new [chat](../resources/chat.md) object.|
|[Get chat](../api/chat-get.md)|[chat](../resources/chat.md)|Read the properties and relationships of a [chat](../resources/chat.md) object.|
|[Update chat](../api/chat-update.md)|[chat](../resources/chat.md)|Update the properties of a [chat](../resources/chat.md) object.|
|[Delete chat](../api/chat-delete.md)|None|Deletes a [chat](../resources/chat.md) object.|
|[sendActivityNotification](../api/chat-sendactivitynotification.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|chatType|chatType|**TODO: Add Description**. The possible values are: `oneOnOne`, `group`, `meeting`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|onlineMeetingInfo|[teamworkOnlineMeetingInfo](../resources/teamworkonlinemeetinginfo.md)|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|topic|String|**TODO: Add Description**|
|viewpoint|[chatViewpoint](../resources/chatviewpoint.md)|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|installedApps|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|**TODO: Add Description**|
|lastMessagePreview|[chatMessageInfo](../resources/chatmessageinfo.md)|**TODO: Add Description**|
|members|[conversationMember](../resources/conversationmember.md) collection|**TODO: Add Description**|
|messages|[chatMessage](../resources/chatmessage.md) collection|**TODO: Add Description**|
|operations|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection|**TODO: Add Description**|
|permissionGrants|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection|**TODO: Add Description**|
|tabs|[teamsTab](../resources/teamstab.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chat",
  "id": "String (identifier)",
  "chatType": "String",
  "createdDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "onlineMeetingInfo": {
    "@odata.type": "microsoft.graph.teamworkOnlineMeetingInfo"
  },
  "tenantId": "String",
  "topic": "String",
  "viewpoint": {
    "@odata.type": "microsoft.graph.chatViewpoint"
  },
  "webUrl": "String"
}
```

