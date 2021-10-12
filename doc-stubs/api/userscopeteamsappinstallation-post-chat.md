---
title: "Add chat"
description: "Add chat by posting to the chat collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add chat
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add chat by posting to the chat collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatsId}/installedApps/{teamsAppInstallationId}/chat/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.

You can specify the following properties when creating a **chat**.

|Property|Type|Description|
|:---|:---|:---|
|tenantId|String|**TODO: Add Description** Optional.|
|topic|String|**TODO: Add Description** Optional.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|chatType|chatType|**TODO: Add Description**. The possible values are: `oneOnOne`, `group`, `meeting`, `unknownFutureValue`. Required.|
|webUrl|String|**TODO: Add Description** Optional.|
|viewpoint|[Microsoft.Teams.GraphSvc.chatViewpoint](../resources/chatviewpoint.md)|**TODO: Add Description** Optional.|
|onlineMeetingInfo|[Microsoft.Teams.GraphSvc.teamworkOnlineMeetingInfo](../resources/teamworkonlinemeetinginfo.md)|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `204 No Content` response code and a [chat](../resources/chat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_chat_from_chats"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatsId}/installedApps/{teamsAppInstallationId}/chat/$ref
Content-Type: application/json
Content-length: 370

{
  "@odata.type": "#Microsoft.Teams.GraphSvc.chat",
  "tenantId": "String",
  "topic": "String",
  "lastUpdatedDateTime": "String (timestamp)",
  "chatType": "String",
  "webUrl": "String",
  "viewpoint": {
    "@odata.type": "microsoft.graph.chatViewpoint"
  },
  "onlineMeetingInfo": {
    "@odata.type": "microsoft.graph.teamworkOnlineMeetingInfo"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.Teams.GraphSvc.chat"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#Microsoft.Teams.GraphSvc.chat",
  "id": "076cf76a-f76a-076c-6af7-6c076af76c07",
  "tenantId": "String",
  "topic": "String",
  "createdDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "chatType": "String",
  "webUrl": "String",
  "viewpoint": {
    "@odata.type": "microsoft.graph.chatViewpoint"
  },
  "onlineMeetingInfo": {
    "@odata.type": "microsoft.graph.teamworkOnlineMeetingInfo"
  }
}
```

