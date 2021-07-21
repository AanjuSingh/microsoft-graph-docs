---
title: "Create openIdConnectIdentityProvider"
description: "Create a new openIdConnectIdentityProvider object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create openIdConnectIdentityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) object.

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
POST ** Collection URI for microsoft.graph.openIdConnectIdentityProvider not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) object.

The following table shows the properties that are required when you create the [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [identityProviderBase](../resources/identityproviderbase.md)|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|**TODO: Add Description**|
|clientId|String|**TODO: Add Description**|
|clientSecret|String|**TODO: Add Description**|
|domainHint|String|**TODO: Add Description**|
|metadataUrl|String|**TODO: Add Description**|
|responseMode|openIdConnectResponseMode|**TODO: Add Description**. Possible values are: `form_post`, `query`, `unknownFutureValue`.|
|responseType|openIdConnectResponseTypes|**TODO: Add Description**. Possible values are: `code`, `id_token`, `token`.|
|scope|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_openidconnectidentityprovider_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.openIdConnectIdentityProvider not found
Content-Type: application/json
Content-length: 368

{
  "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
  "displayName": "String",
  "claimsMapping": {
    "@odata.type": "microsoft.graph.claimsMapping"
  },
  "clientId": "String",
  "clientSecret": "String",
  "domainHint": "String",
  "metadataUrl": "String",
  "responseMode": "String",
  "responseType": "String",
  "scope": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
  "id": "f44f1168-1168-f44f-6811-4ff468114ff4",
  "displayName": "String",
  "claimsMapping": {
    "@odata.type": "microsoft.graph.claimsMapping"
  },
  "clientId": "String",
  "clientSecret": "String",
  "domainHint": "String",
  "metadataUrl": "String",
  "responseMode": "String",
  "responseType": "String",
  "scope": "String"
}
```

