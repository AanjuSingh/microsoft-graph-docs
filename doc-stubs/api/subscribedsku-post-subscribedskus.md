---
title: "Create subscribedSku"
description: "Create a new subscribedSku object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create subscribedSku
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [subscribedSku](../resources/subscribedsku.md) object.

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
POST /subscribedSkus
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [subscribedSku](../resources/subscribedsku.md) object.

The following table shows the properties that are required when you create the [subscribedSku](../resources/subscribedsku.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appliesTo|String|**TODO: Add Description**|
|capabilityStatus|String|**TODO: Add Description**|
|consumedUnits|Int32|**TODO: Add Description**|
|prepaidUnits|[licenseUnitsDetail](../resources/licenseunitsdetail.md)|**TODO: Add Description**|
|servicePlans|[servicePlanInfo](../resources/serviceplaninfo.md) collection|**TODO: Add Description**|
|skuId|Guid|**TODO: Add Description**|
|skuPartNumber|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [subscribedSku](../resources/subscribedsku.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_subscribedsku_from_subscribedskus"
}
-->
``` http
POST https://graph.microsoft.com/beta/subscribedSkus
Content-Type: application/json
Content-length: 376

{
  "@odata.type": "#microsoft.graph.subscribedSku",
  "appliesTo": "String",
  "capabilityStatus": "String",
  "consumedUnits": "Integer",
  "prepaidUnits": {
    "@odata.type": "microsoft.graph.licenseUnitsDetail"
  },
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.subscribedSku",
  "id": "a7890dde-0dde-a789-de0d-89a7de0d89a7",
  "appliesTo": "String",
  "capabilityStatus": "String",
  "consumedUnits": "Integer",
  "prepaidUnits": {
    "@odata.type": "microsoft.graph.licenseUnitsDetail"
  },
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String"
}
```

