---
title: "Create socialIdentityProvider"
description: "Create a new socialIdentityProvider object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create socialIdentityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [socialIdentityProvider](../resources/socialidentityprovider.md) object.

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
POST ** Collection URI for microsoft.graph.socialIdentityProvider not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [socialIdentityProvider](../resources/socialidentityprovider.md) object.

The following table shows the properties that are required when you create the [socialIdentityProvider](../resources/socialidentityprovider.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [identityProviderBase](../resources/identityproviderbase.md)|
|clientId|String|**TODO: Add Description**|
|clientSecret|String|**TODO: Add Description**|
|identityProviderType|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [socialIdentityProvider](../resources/socialidentityprovider.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_socialidentityprovider_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.socialIdentityProvider not found
Content-Type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.socialIdentityProvider",
  "displayName": "String",
  "clientId": "String",
  "clientSecret": "String",
  "identityProviderType": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.socialIdentityProvider"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.socialIdentityProvider",
  "id": "c71311e0-11e0-c713-e011-13c7e01113c7",
  "displayName": "String",
  "clientId": "String",
  "clientSecret": "String",
  "identityProviderType": "String"
}
```

