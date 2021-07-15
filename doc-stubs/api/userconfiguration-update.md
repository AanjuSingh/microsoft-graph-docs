---
title: "Update userConfiguration"
description: "Update the properties of a userConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [userConfiguration](../resources/userconfiguration.md) object.

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
PATCH /me/mailFolders/{mailFolderId}/userConfigurations/{userConfigurationId}
PATCH /users/{usersId}/mailFolders/{mailFolderId}/userConfigurations/{userConfigurationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userConfiguration](../resources/userconfiguration.md) object.

The following table shows the properties that are required when you update the [userConfiguration](../resources/userconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|binaryData|Binary|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [userConfiguration](../resources/userconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/mailFolders/{mailFolderId}/userConfigurations/{userConfigurationId}
Content-Type: application/json
Content-length: 86

{
  "@odata.type": "#microsoft.graph.userConfiguration",
  "binaryData": "Binary"
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
  "@odata.type": "#microsoft.graph.userConfiguration",
  "id": "3afba498-a498-3afb-98a4-fb3a98a4fb3a",
  "binaryData": "Binary"
}
```

