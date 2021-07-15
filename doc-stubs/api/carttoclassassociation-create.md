---
title: "Create cartToClassAssociation"
description: "Create a new cartToClassAssociation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create cartToClassAssociation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [cartToClassAssociation](../resources/carttoclassassociation.md) object.

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
POST /deviceManagement/cartToClassAssociations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [cartToClassAssociation](../resources/carttoclassassociation.md) object.

The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/carttoclassassociation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|classroomIds|String collection|Identifiers of classrooms to be associated with device carts.|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the CartToClassAssociation.|
|deviceCartIds|String collection|Identifiers of device carts to be associated with classes.|
|displayName|String|Admin provided name of the device configuration.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|version|Int32|Version of the CartToClassAssociation.|



## Response

If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/carttoclassassociation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_carttoclassassociation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-Type: application/json
Content-length: 228

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "classroomIds": [
    "String"
  ],
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "displayName": "String",
  "version": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cartToClassAssociation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "eb431f2e-1f2e-eb43-2e1f-43eb2e1f43eb",
  "classroomIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "version": "Integer"
}
```

