---
title: "Update itemInsightsSettings"
description: "Update the properties of an itemInsightsSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update itemInsightsSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [itemInsightsSettings](../resources/iteminsightssettings.md) object.

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
PATCH /organization/{organizationId}/settings/itemInsights
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [itemInsightsSettings](../resources/iteminsightssettings.md) object.

The following table shows the properties that are required when you update the [itemInsightsSettings](../resources/iteminsightssettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|disabledForGroup|String|**TODO: Add Description**|
|isEnabledInOrganization|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_iteminsightssettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-Type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.itemInsightsSettings",
  "disabledForGroup": "String",
  "isEnabledInOrganization": "Boolean"
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
  "@odata.type": "#microsoft.graph.itemInsightsSettings",
  "id": "9cf09b35-9b35-9cf0-359b-f09c359bf09c",
  "disabledForGroup": "String",
  "isEnabledInOrganization": "Boolean"
}
```

