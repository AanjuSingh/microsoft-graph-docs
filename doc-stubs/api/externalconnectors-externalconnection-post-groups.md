---
title: "Create externalGroup"
description: "Create a new externalGroup object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create externalGroup
Namespace: microsoft.graph.externalConnectors



Create a new externalGroup object.

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
POST /connections/{connectionsId}/groups
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [externalGroup](../resources/externalconnectors-externalgroup.md) object.

The following table shows the properties that are required when you create the [externalGroup](../resources/externalconnectors-externalgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/externalconnectors-entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [externalGroup](../resources/externalconnectors-externalgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/connections/{connectionsId}/groups
Content-Type: application/json
Content-length: 130

{
  "@odata.type": "#microsoft.graph.externalConnectors.externalGroup",
  "displayName": "String",
  "description": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalConnectors.externalGroup",
  "id": "b8aab634-b634-b8aa-34b6-aab834b6aab8",
  "displayName": "String",
  "description": "String"
}
```

