---
title: "Create deviceManagementResourceAccessProfileBase"
description: "Create a new deviceManagementResourceAccessProfileBase object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceManagementResourceAccessProfileBase
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new deviceManagementResourceAccessProfileBase object.

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
POST /deviceManagement/resourceAccessProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementResourceAccessProfileBase](../resources/devicemanagementresourceaccessprofilebase.md) object.

The following table shows the properties that are required when you create the [deviceManagementResourceAccessProfileBase](../resources/devicemanagementresourceaccessprofilebase.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset|DateTime profile was created|
|description|String|Profile description|
|displayName|String|Profile display name|
|lastModifiedDateTime|DateTimeOffset|DateTime profile was last modified|
|roleScopeTagIds|String collection|Scope Tags|
|version|Int32|Version of the profile|



## Response

If successful, this method returns a `201 Created` response code and a [deviceManagementResourceAccessProfileBase](../resources/devicemanagementresourceaccessprofilebase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementresourceaccessprofilebase_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
Content-Type: application/json
Content-length: 253

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileBase",
  "creationDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementResourceAccessProfileBase"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileBase",
  "id": "df99e712-e712-df99-12e7-99df12e799df",
  "creationDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "Integer"
}
```

