---
title: "List locationManagementConditions"
description: "Get a list of the locationManagementCondition objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List locationManagementConditions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [locationManagementCondition](../resources/locationmanagementcondition.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.locationManagementCondition not found
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

If successful, this method returns a `200 OK` response code and a collection of [locationManagementCondition](../resources/locationmanagementcondition.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_locationmanagementcondition"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.locationManagementCondition not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.locationManagementCondition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.locationManagementCondition",
      "id": "b51a60c6-60c6-b51a-c660-1ab5c6601ab5",
      "applicablePlatforms": [
        "String"
      ],
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "displayName": "String",
      "eTag": "String",
      "modifiedDateTime": "String (timestamp)",
      "uniqueName": "String"
    }
  ]
}
```

