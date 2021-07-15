---
title: "Create temporaryAccessPassAuthenticationMethod"
description: "Create a new temporaryAccessPassAuthenticationMethod object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create temporaryAccessPassAuthenticationMethod
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.

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
POST /me/authentication/temporaryAccessPassMethods
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.

The following table shows the properties that are required when you create the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|isUsable|Boolean|**TODO: Add Description**|
|isUsableOnce|Boolean|**TODO: Add Description**|
|lifetimeInMinutes|Int32|**TODO: Add Description**|
|methodUsabilityReason|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|temporaryAccessPass|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_temporaryaccesspassauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/authentication/temporaryAccessPassMethods
Content-Type: application/json
Content-length: 288

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "isUsable": "Boolean",
  "isUsableOnce": "Boolean",
  "lifetimeInMinutes": "Integer",
  "methodUsabilityReason": "String",
  "startDateTime": "String (timestamp)",
  "temporaryAccessPass": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "id": "a5402166-2166-a540-6621-40a5662140a5",
  "createdDateTime": "String (timestamp)",
  "isUsable": "Boolean",
  "isUsableOnce": "Boolean",
  "lifetimeInMinutes": "Integer",
  "methodUsabilityReason": "String",
  "startDateTime": "String (timestamp)",
  "temporaryAccessPass": "String"
}
```

