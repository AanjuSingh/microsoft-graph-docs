---
title: "Create fido2AuthenticationMethod"
description: "Create a new fido2AuthenticationMethod object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create fido2AuthenticationMethod
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object.

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
POST /me/authentication/fido2Methods
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object.

The following table shows the properties that are required when you create the [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|aaGuid|String|**TODO: Add Description**|
|attestationCertificates|String collection|**TODO: Add Description**|
|attestationLevel|attestationLevel|**TODO: Add Description**. Possible values are: `attested`, `notAttested`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_fido2authenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/authentication/fido2Methods
Content-Type: application/json
Content-length: 270

{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
  "aaGuid": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String",
  "creationDateTime": "String (timestamp)",
  "displayName": "String",
  "model": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
  "id": "bd96c925-c925-bd96-25c9-96bd25c996bd",
  "aaGuid": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String",
  "createdDateTime": "String (timestamp)",
  "creationDateTime": "String (timestamp)",
  "displayName": "String",
  "model": "String"
}
```

