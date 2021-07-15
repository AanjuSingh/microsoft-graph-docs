---
title: "Update sideLoadingKey"
description: "Update the properties of a sideLoadingKey object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update sideLoadingKey
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [sideLoadingKey](../resources/sideloadingkey.md) object.

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
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [sideLoadingKey](../resources/sideloadingkey.md) object.

The following table shows the properties that are required when you update the [sideLoadingKey](../resources/sideloadingkey.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|Side Loading Key description displayed to the ITPro Admins..|
|displayName|String|Side Loading Key Name displayed to the ITPro Admins.|
|lastUpdatedDateTime|String|Side Loading Key Last Updated Date displayed to the ITPro Admins.|
|totalActivation|Int32|Side Loading Key Total Activation displayed to the ITPro Admins.|
|value|String|Side Loading Key Value, it is 5x5 value, seperated by hiphens.|



## Response

If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/sideloadingkey.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_sideloadingkey"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-Type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "description": "String",
  "displayName": "String",
  "lastUpdatedDateTime": "String",
  "totalActivation": "Integer",
  "value": "String"
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
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "c86c842a-842a-c86c-2a84-6cc82a846cc8",
  "description": "String",
  "displayName": "String",
  "lastUpdatedDateTime": "String",
  "totalActivation": "Integer",
  "value": "String"
}
```

