---
title: "Create userScopeTeamsAppInstallation"
description: "Create a new userScopeTeamsAppInstallation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userScopeTeamsAppInstallation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new userScopeTeamsAppInstallation object.

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
POST /users/{usersId}/teamwork/installedApps
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userScopeTeamsAppInstallation](../resources/userscopeteamsappinstallation.md) object.

The following table shows the properties that are required when you create the [userScopeTeamsAppInstallation](../resources/userscopeteamsappinstallation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response

If successful, this method returns a `201 Created` response code and a [userScopeTeamsAppInstallation](../resources/userscopeteamsappinstallation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userscopeteamsappinstallation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/teamwork/installedApps
Content-Type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.userScopeTeamsAppInstallation"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userScopeTeamsAppInstallation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.userScopeTeamsAppInstallation",
  "id": "7adc2b18-2b18-7adc-182b-dc7a182bdc7a"
}
```

