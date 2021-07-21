---
title: "Update microsoftAuthenticatorAuthenticationMethodTarget"
description: "Update the properties of a microsoftAuthenticatorAuthenticationMethodTarget object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update microsoftAuthenticatorAuthenticationMethodTarget
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) object.

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
PATCH /microsoftAuthenticatorAuthenticationMethodConfiguration/includeTargets/{microsoftAuthenticatorAuthenticationMethodTargetId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) object.

The following table shows the properties that are required when you update the [microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isRegistrationRequired|Boolean|**TODO: Add Description** Inherited from [authenticationMethodTarget](../resources/authenticationmethodtarget.md)|
|targetType|authenticationMethodTargetType|**TODO: Add Description** Inherited from [authenticationMethodTarget](../resources/authenticationmethodtarget.md). Possible values are: `user`, `group`, `unknownFutureValue`.|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|**TODO: Add Description**. Possible values are: `deviceBasedPush`, `push`, `any`.|
|featureSettings|authenticatorAppFeatureSettings|**TODO: Add Description**. Possible values are: `requireNumberMatching`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_microsoftauthenticatorauthenticationmethodtarget"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/microsoftAuthenticatorAuthenticationMethodConfiguration/includeTargets/{microsoftAuthenticatorAuthenticationMethodTargetId}
Content-Type: application/json
Content-length: 224

{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "isRegistrationRequired": "Boolean",
  "targetType": "String",
  "authenticationMode": "String",
  "featureSettings": "String"
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
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "id": "cb0c89d9-89d9-cb0c-d989-0ccbd9890ccb",
  "isRegistrationRequired": "Boolean",
  "targetType": "String",
  "authenticationMode": "String",
  "featureSettings": "String"
}
```

