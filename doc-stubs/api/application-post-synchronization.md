---
title: "Create synchronization"
description: "Create a new synchronization object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create synchronization
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new synchronization object.

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
POST /applications/{applicationsId}/synchronization
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [synchronization](../resources/synchronization.md) object.

The following table shows the properties that are required when you create the [synchronization](../resources/synchronization.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|secrets|[synchronizationSecretKeyStringValuePair](../resources/synchronizationsecretkeystringvaluepair.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [synchronization](../resources/synchronization.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_synchronization_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization
Content-Type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.synchronization",
  "secrets": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronization"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.synchronization",
  "id": "e4a1fb12-fb12-e4a1-12fb-a1e412fba1e4",
  "secrets": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```

