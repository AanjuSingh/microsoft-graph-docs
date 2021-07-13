---
title: "Create emailAppUsageVersionsUserCounts"
description: "Create a new emailAppUsageVersionsUserCounts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create emailAppUsageVersionsUserCounts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.emailAppUsageVersionsUserCounts not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object.

The following table shows the properties that are required when you create the [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|outlook2007|Int64|**TODO: Add Description**|
|outlook2010|Int64|**TODO: Add Description**|
|outlook2013|Int64|**TODO: Add Description**|
|outlook2016|Int64|**TODO: Add Description**|
|outlook2019|Int64|**TODO: Add Description**|
|outlookM365|Int64|**TODO: Add Description**|
|reportPeriod|String|**TODO: Add Description**|
|reportRefreshDate|Date|**TODO: Add Description**|
|undetermined|Int64|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_emailappusageversionsusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.emailAppUsageVersionsUserCounts not found
Content-Type: application/json
Content-length: 338

{
  "@odata.type": "#microsoft.graph.emailAppUsageVersionsUserCounts",
  "outlook2007": "Integer",
  "outlook2010": "Integer",
  "outlook2013": "Integer",
  "outlook2016": "Integer",
  "outlook2019": "Integer",
  "outlookM365": "Integer",
  "reportPeriod": "String",
  "reportRefreshDate": "Date",
  "undetermined": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.emailAppUsageVersionsUserCounts",
  "id": "0f1eb526-b526-0f1e-26b5-1e0f26b51e0f",
  "outlook2007": "Integer",
  "outlook2010": "Integer",
  "outlook2013": "Integer",
  "outlook2016": "Integer",
  "outlook2019": "Integer",
  "outlookM365": "Integer",
  "reportPeriod": "String",
  "reportRefreshDate": "Date",
  "undetermined": "Integer"
}
```

