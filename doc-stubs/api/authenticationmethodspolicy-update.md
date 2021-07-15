---
title: "Update authenticationMethodsPolicy"
description: "Update the properties of an authenticationMethodsPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update authenticationMethodsPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.

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
PATCH /authenticationMethodsPolicy
PATCH /policies/authenticationMethodsPolicy
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.

The following table shows the properties that are required when you update the [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|policyVersion|String|**TODO: Add Description**|
|reconfirmationInDays|Int32|**TODO: Add Description**|
|registrationEnforcement|[registrationEnforcement](../resources/registrationenforcement.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_authenticationmethodspolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/authenticationMethodsPolicy
Content-Type: application/json
Content-length: 293

{
  "@odata.type": "#microsoft.graph.authenticationMethodsPolicy",
  "description": "String",
  "displayName": "String",
  "policyVersion": "String",
  "reconfirmationInDays": "Integer",
  "registrationEnforcement": {
    "@odata.type": "microsoft.graph.registrationEnforcement"
  }
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
  "@odata.type": "#microsoft.graph.authenticationMethodsPolicy",
  "id": "a537ac15-ac15-a537-15ac-37a515ac37a5",
  "description": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyVersion": "String",
  "reconfirmationInDays": "Integer",
  "registrationEnforcement": {
    "@odata.type": "microsoft.graph.registrationEnforcement"
  }
}
```

