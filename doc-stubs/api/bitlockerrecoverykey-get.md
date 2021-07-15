---
title: "Get bitlockerRecoveryKey"
description: "Read the properties and relationships of a bitlockerRecoveryKey object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get bitlockerRecoveryKey
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.

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
GET /me/informationProtection/bitlocker/recoveryKeys/{bitlockerRecoveryKeyId}
GET /users/{usersId}/informationProtection/bitlocker/recoveryKeys/{bitlockerRecoveryKeyId}
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

If successful, this method returns a `200 OK` response code and a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/informationProtection/bitlocker/recoveryKeys/{bitlockerRecoveryKeyId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "bce76dbf-6dbf-bce7-bf6d-e7bcbf6de7bc",
    "createdDateTime": "String (timestamp)",
    "deviceId": "String",
    "key": "String",
    "volumeType": "String"
  }
}
```

