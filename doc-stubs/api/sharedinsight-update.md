---
title: "Update sharedInsight"
description: "Update the properties of a sharedInsight object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update sharedInsight
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [sharedInsight](../resources/sharedinsight.md) object.

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
PATCH /officeGraphInsights/shared/{sharedInsightId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [sharedInsight](../resources/sharedinsight.md) object.

The following table shows the properties that are required when you update the [sharedInsight](../resources/sharedinsight.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastShared|[sharingDetail](../resources/sharingdetail.md)|**TODO: Add Description**|
|resourceReference|[resourceReference](../resources/resourcereference.md)|**TODO: Add Description**|
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)|**TODO: Add Description**|
|sharingHistory|[sharingDetail](../resources/sharingdetail.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [sharedInsight](../resources/sharedinsight.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_sharedinsight"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/officeGraphInsights/shared/{sharedInsightId}
Content-Type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.sharedInsight",
  "lastShared": {
    "@odata.type": "microsoft.graph.sharingDetail"
  },
  "resourceReference": {
    "@odata.type": "microsoft.graph.resourceReference"
  },
  "resourceVisualization": {
    "@odata.type": "microsoft.graph.resourceVisualization"
  },
  "sharingHistory": [
    {
      "@odata.type": "microsoft.graph.sharingDetail"
    }
  ]
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
  "@odata.type": "#microsoft.graph.sharedInsight",
  "id": "1f017969-7969-1f01-6979-011f6979011f",
  "lastShared": {
    "@odata.type": "microsoft.graph.sharingDetail"
  },
  "resourceReference": {
    "@odata.type": "microsoft.graph.resourceReference"
  },
  "resourceVisualization": {
    "@odata.type": "microsoft.graph.resourceVisualization"
  },
  "sharingHistory": [
    {
      "@odata.type": "microsoft.graph.sharingDetail"
    }
  ]
}
```

