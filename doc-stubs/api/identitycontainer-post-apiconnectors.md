---
title: "Create identityApiConnector"
description: "Create a new identityApiConnector object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create identityApiConnector
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new identityApiConnector object.

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
POST /identity/apiConnectors
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.

The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|authenticationConfiguration|[apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|targetUrl|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identity/apiConnectors
Content-Type: application/json
Content-length: 231

{
  "@odata.type": "#microsoft.graph.identityApiConnector",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
  },
  "displayName": "String",
  "targetUrl": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.identityApiConnector",
  "id": "1eaf46ca-46ca-1eaf-ca46-af1eca46af1e",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
  },
  "displayName": "String",
  "targetUrl": "String"
}
```

