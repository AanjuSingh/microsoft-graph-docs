---
title: "List accessPackageAssignmentRequests"
description: "Get a list of the accessPackageAssignmentRequest objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List accessPackageAssignmentRequests
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects and their properties.

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
GET /accessPackageAssignmentRequests
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

If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_accesspackageassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignmentRequests
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageAssignmentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageAssignmentRequest",
      "answers": [
        {
          "@odata.type": "microsoft.graph.accessPackageAnswerString"
        }
      ],
      "completedDate": "String (timestamp)",
      "createdDateTime": "String (timestamp)",
      "expirationDateTime": "String (timestamp)",
      "id": "9700ab8f-ab8f-9700-8fab-00978fab0097",
      "isValidationOnly": "Boolean",
      "justification": "String",
      "requestState": "String",
      "requestStatus": "String",
      "requestType": "String",
      "schedule": {
        "@odata.type": "microsoft.graph.requestSchedule"
      }
    }
  ]
}
```

