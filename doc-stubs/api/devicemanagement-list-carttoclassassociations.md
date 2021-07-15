---
title: "List cartToClassAssociations"
description: "Get the cartToClassAssociation resources from the cartToClassAssociations navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List cartToClassAssociations
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the cartToClassAssociation resources from the cartToClassAssociations navigation property.

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
GET /deviceManagement/cartToClassAssociations
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

If successful, this method returns a `200 OK` response code and a collection of [cartToClassAssociation](../resources/carttoclassassociation.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_carttoclassassociation"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cartToClassAssociation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cartToClassAssociation",
      "id": "eb431f2e-1f2e-eb43-2e1f-43eb2e1f43eb",
      "classroomIds": [
        "String"
      ],
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "deviceCartIds": [
        "String"
      ],
      "displayName": "String",
      "lastModifiedDateTime": "String (timestamp)",
      "version": "Integer"
    }
  ]
}
```

