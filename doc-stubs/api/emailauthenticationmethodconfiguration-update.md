---
title: "Update emailAuthenticationMethodConfiguration"
description: "Update the properties of an emailAuthenticationMethodConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update emailAuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object.

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
PATCH /emailAuthenticationMethodConfiguration
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object.

The following table shows the properties that are required when you update the [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|state|authenticationMethodState|**TODO: Add Description** Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md). Possible values are: `enabled`, `disabled`.|
|allowExternalIdToUseEmailOtp|externalEmailOtpState|**TODO: Add Description**. Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/emailAuthenticationMethodConfiguration
Content-Type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "state": "String",
  "allowExternalIdToUseEmailOtp": "String"
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
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "id": "1191a18b-a18b-1191-8ba1-91118ba19111",
  "state": "String",
  "allowExternalIdToUseEmailOtp": "String"
}
```

