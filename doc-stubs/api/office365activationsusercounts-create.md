---
title: "Create office365ActivationsUserCounts"
description: "Create a new office365ActivationsUserCounts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create office365ActivationsUserCounts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.office365ActivationsUserCounts not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) object.

The following table shows the properties that are required when you create the [office365ActivationsUserCounts](../resources/office365activationsusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activated|Int64|**TODO: Add Description**|
|assigned|Int64|**TODO: Add Description**|
|productType|String|**TODO: Add Description**|
|reportRefreshDate|Date|**TODO: Add Description**|
|sharedComputerActivation|Int64|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_office365activationsusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.office365ActivationsUserCounts not found
Content-Type: application/json
Content-length: 227

{
  "@odata.type": "#microsoft.graph.office365ActivationsUserCounts",
  "activated": "Integer",
  "assigned": "Integer",
  "productType": "String",
  "reportRefreshDate": "Date",
  "sharedComputerActivation": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.office365ActivationsUserCounts",
  "id": "dd6dcbbd-cbbd-dd6d-bdcb-6dddbdcb6ddd",
  "activated": "Integer",
  "assigned": "Integer",
  "productType": "String",
  "reportRefreshDate": "Date",
  "sharedComputerActivation": "Integer"
}
```

