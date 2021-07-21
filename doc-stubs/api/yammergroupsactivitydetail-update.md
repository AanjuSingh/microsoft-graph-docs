---
title: "Update yammerGroupsActivityDetail"
description: "Update the properties of a yammerGroupsActivityDetail object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update yammerGroupsActivityDetail
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object.

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
PATCH /yammerGroupsActivityDetail
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object.

The following table shows the properties that are required when you update the [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|groupDisplayName|String|**TODO: Add Description**|
|groupType|String|**TODO: Add Description**|
|isDeleted|Boolean|**TODO: Add Description**|
|lastActivityDate|Date|**TODO: Add Description**|
|likedCount|Int64|**TODO: Add Description**|
|memberCount|Int64|**TODO: Add Description**|
|networkDisplayName|String|**TODO: Add Description**|
|office365Connected|Boolean|**TODO: Add Description**|
|ownerPrincipalName|String|**TODO: Add Description**|
|postedCount|Int64|**TODO: Add Description**|
|readCount|Int64|**TODO: Add Description**|
|reportPeriod|String|**TODO: Add Description**|
|reportRefreshDate|Date|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_yammergroupsactivitydetail"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/yammerGroupsActivityDetail
Content-Type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityDetail",
  "groupDisplayName": "String",
  "groupType": "String",
  "isDeleted": "Boolean",
  "lastActivityDate": "Date",
  "likedCount": "Integer",
  "memberCount": "Integer",
  "networkDisplayName": "String",
  "office365Connected": "Boolean",
  "ownerPrincipalName": "String",
  "postedCount": "Integer",
  "readCount": "Integer",
  "reportPeriod": "String",
  "reportRefreshDate": "Date"
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
  "@odata.type": "#microsoft.graph.yammerGroupsActivityDetail",
  "id": "c41e3195-3195-c41e-9531-1ec495311ec4",
  "groupDisplayName": "String",
  "groupType": "String",
  "isDeleted": "Boolean",
  "lastActivityDate": "Date",
  "likedCount": "Integer",
  "memberCount": "Integer",
  "networkDisplayName": "String",
  "office365Connected": "Boolean",
  "ownerPrincipalName": "String",
  "postedCount": "Integer",
  "readCount": "Integer",
  "reportPeriod": "String",
  "reportRefreshDate": "Date"
}
```

