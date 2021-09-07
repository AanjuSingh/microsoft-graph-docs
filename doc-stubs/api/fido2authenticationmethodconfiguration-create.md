---
title: "Create fido2AuthenticationMethodConfiguration"
description: "Create a new fido2AuthenticationMethodConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create fido2AuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object.

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
POST ** Collection URI for microsoft.authMethodPolicy.fido2AuthenticationMethodConfiguration not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object.

The following table shows the properties that are required when you create the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)|
|state|authenticationMethodState|**TODO: Add Description** Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md). The possible values are: `enabled`, `disabled`.|
|isSelfServiceRegistrationAllowed|Boolean|**TODO: Add Description**|
|isAttestationEnforced|Boolean|**TODO: Add Description**|
|keyRestrictions|[microsoft.authMethodPolicy.fido2KeyRestrictions](../resources/fido2keyrestrictions.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_fido2authenticationmethodconfiguration_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.authMethodPolicy.fido2AuthenticationMethodConfiguration not found
Content-Type: application/json
Content-length: 291

{
  "@odata.type": "#microsoft.authMethodPolicy.fido2AuthenticationMethodConfiguration",
  "state": "String",
  "isSelfServiceRegistrationAllowed": "Boolean",
  "isAttestationEnforced": "Boolean",
  "keyRestrictions": {
    "@odata.type": "microsoft.graph.fido2KeyRestrictions"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.authMethodPolicy.fido2AuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.authMethodPolicy.fido2AuthenticationMethodConfiguration",
  "id": "4bc2eb8a-eb8a-4bc2-8aeb-c24b8aebc24b",
  "state": "String",
  "isSelfServiceRegistrationAllowed": "Boolean",
  "isAttestationEnforced": "Boolean",
  "keyRestrictions": {
    "@odata.type": "microsoft.graph.fido2KeyRestrictions"
  }
}
```

