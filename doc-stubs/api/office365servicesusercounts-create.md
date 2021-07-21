---
title: "Create office365ServicesUserCounts"
description: "Create a new office365ServicesUserCounts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create office365ServicesUserCounts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.office365ServicesUserCounts not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object.

The following table shows the properties that are required when you create the [office365ServicesUserCounts](../resources/office365servicesusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|exchangeActive|Int64|**TODO: Add Description**|
|exchangeInactive|Int64|**TODO: Add Description**|
|office365Active|Int64|**TODO: Add Description**|
|office365Inactive|Int64|**TODO: Add Description**|
|oneDriveActive|Int64|**TODO: Add Description**|
|oneDriveInactive|Int64|**TODO: Add Description**|
|reportPeriod|String|**TODO: Add Description**|
|reportRefreshDate|Date|**TODO: Add Description**|
|sharePointActive|Int64|**TODO: Add Description**|
|sharePointInactive|Int64|**TODO: Add Description**|
|skypeForBusinessActive|Int64|**TODO: Add Description**|
|skypeForBusinessInactive|Int64|**TODO: Add Description**|
|teamsActive|Int64|**TODO: Add Description**|
|teamsInactive|Int64|**TODO: Add Description**|
|yammerActive|Int64|**TODO: Add Description**|
|yammerInactive|Int64|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_office365servicesusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.office365ServicesUserCounts not found
Content-Type: application/json
Content-length: 604

{
  "@odata.type": "#microsoft.graph.office365ServicesUserCounts",
  "exchangeActive": "Integer",
  "exchangeInactive": "Integer",
  "office365Active": "Integer",
  "office365Inactive": "Integer",
  "oneDriveActive": "Integer",
  "oneDriveInactive": "Integer",
  "reportPeriod": "String",
  "reportRefreshDate": "Date",
  "sharePointActive": "Integer",
  "sharePointInactive": "Integer",
  "skypeForBusinessActive": "Integer",
  "skypeForBusinessInactive": "Integer",
  "teamsActive": "Integer",
  "teamsInactive": "Integer",
  "yammerActive": "Integer",
  "yammerInactive": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.office365ServicesUserCounts",
  "id": "c4093496-3496-c409-9634-09c4963409c4",
  "exchangeActive": "Integer",
  "exchangeInactive": "Integer",
  "office365Active": "Integer",
  "office365Inactive": "Integer",
  "oneDriveActive": "Integer",
  "oneDriveInactive": "Integer",
  "reportPeriod": "String",
  "reportRefreshDate": "Date",
  "sharePointActive": "Integer",
  "sharePointInactive": "Integer",
  "skypeForBusinessActive": "Integer",
  "skypeForBusinessInactive": "Integer",
  "teamsActive": "Integer",
  "teamsInactive": "Integer",
  "yammerActive": "Integer",
  "yammerInactive": "Integer"
}
```

