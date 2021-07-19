---
title: "List calls"
description: "Get a list of the call objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List calls
Namespace: microsoft.graph



Get a list of the [call](../resources/call.md) objects and their properties.

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
GET /communications/calls
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [call](../resources/call.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_call"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/communications/calls
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.call)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.call",
      "id": "0ecdb444-b444-0ecd-44b4-cd0e44b4cd0e",
      "state": "String",
      "mediaState": {
        "@odata.type": "microsoft.graph.callMediaState"
      },
      "resultInfo": {
        "@odata.type": "microsoft.graph.resultInfo"
      },
      "direction": "String",
      "subject": "String",
      "callbackUri": "String",
      "callRoutes": [
        {
          "@odata.type": "microsoft.graph.callRoute"
        }
      ],
      "source": {
        "@odata.type": "microsoft.graph.participantInfo"
      },
      "targets": [
        {
          "@odata.type": "microsoft.graph.invitationParticipantInfo"
        }
      ],
      "requestedModalities": [
        "String"
      ],
      "mediaConfig": {
        "@odata.type": "microsoft.graph.mediaConfig"
      },
      "chatInfo": {
        "@odata.type": "microsoft.graph.chatInfo"
      },
      "callOptions": {
        "@odata.type": "microsoft.graph.callOptions"
      },
      "meetingInfo": {
        "@odata.type": "microsoft.graph.meetingInfo"
      },
      "transcription": {
        "@odata.type": "microsoft.graph.callTranscriptionInfo"
      },
      "tenantId": "String",
      "myParticipantId": "String",
      "toneInfo": {
        "@odata.type": "microsoft.graph.toneInfo"
      },
      "callChainId": "String",
      "incomingContext": {
        "@odata.type": "microsoft.graph.incomingContext"
      }
    }
  ]
}
```

