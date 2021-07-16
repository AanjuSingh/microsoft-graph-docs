---
title: "Get serviceUpdateMessage"
description: "Read the properties and relationships of a serviceUpdateMessage object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get serviceUpdateMessage
Namespace: microsoft.graph



Read the properties and relationships of a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object.

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
GET /admin/serviceAnnouncement/messages/{serviceUpdateMessageId}
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

If successful, this method returns a `200 OK` response code and a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_serviceupdatemessage"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/admin/serviceAnnouncement/messages/{serviceUpdateMessageId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceUpdateMessage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.serviceUpdateMessage",
    "id": "acafe123-e123-acaf-23e1-afac23e1afac",
    "startDateTime": "String (timestamp)",
    "endDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "title": "String",
    "details": [
      {
        "@odata.type": "microsoft.graph.keyValuePair"
      }
    ],
    "body": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "category": "String",
    "severity": "String",
    "tags": [
      "String"
    ],
    "isMajorChange": "Boolean",
    "actionRequiredByDateTime": "String (timestamp)",
    "services": [
      "String"
    ],
    "viewPoint": {
      "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
    }
  }
}
```

