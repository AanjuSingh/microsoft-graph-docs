---
title: "Update dataSourceContainer"
description: "Update the properties of a dataSourceContainer object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update dataSourceContainer
Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md) object.

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
PATCH /dataSourceContainer
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md) object.

The following table shows the properties that are required when you update the [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/ediscovery-entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|releasedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|dataSourceContainerStatus|**TODO: Add Description**. Possible values are: `Active`, `Released`, `UnknownFutureValue`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_datasourcecontainer"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataSourceContainer
Content-Type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.ediscovery.dataSourceContainer",
  "displayName": "String",
  "releasedDateTime": "String (timestamp)",
  "status": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.ediscovery.dataSourceContainer",
  "id": "add37d1c-7d1c-add3-1c7d-d3ad1c7dd3ad",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "status": "String"
}
```

