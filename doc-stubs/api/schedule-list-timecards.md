---
title: "List timeCards"
description: "Get the timeCard resources from the timeCards navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List timeCards
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the timeCard resources from the timeCards navigation property.

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
GET /teams/{teamsId}/schedule/timeCards
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

If successful, this method returns a `200 OK` response code and a collection of [timeCard](../resources/timecard.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_timecard"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/schedule/timeCards
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.timeCard)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.timeCard",
      "id": "dfdef807-f807-dfde-07f8-dedf07f8dedf",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "String (timestamp)",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "breaks": [
        {
          "@odata.type": "microsoft.graph.timeCardBreak"
        }
      ],
      "clockInEvent": {
        "@odata.type": "microsoft.graph.timeCardEvent"
      },
      "clockOutEvent": {
        "@odata.type": "microsoft.graph.timeCardEvent"
      },
      "confirmedBy": "String",
      "notes": {
        "@odata.type": "microsoft.graph.itemBody"
      },
      "originalEntry": {
        "@odata.type": "microsoft.graph.timeCardEntry"
      },
      "state": "String",
      "userId": "String"
    }
  ]
}
```

