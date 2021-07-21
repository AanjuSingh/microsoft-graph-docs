---
title: "Add administrativeUnit"
description: "Add administrativeUnit by posting to the administrativeUnit collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add administrativeUnit
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add administrativeUnit by posting to the administrativeUnit collection.

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
POST /education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [administrativeUnit](../resources/administrativeunit.md) object.

The following table shows the properties that are required when you create the [administrativeUnit](../resources/administrativeunit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|visibility|String|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit/$ref
Content-Type: application/json
Content-length: 187

{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "visibility": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "id": "3c6e6cb0-6cb0-3c6e-b06c-6e3cb06c6e3c",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "visibility": "String"
}
```

