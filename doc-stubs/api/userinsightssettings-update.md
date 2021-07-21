---
title: "Update userInsightsSettings"
description: "Update the properties of a userInsightsSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userInsightsSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [userInsightsSettings](../resources/userinsightssettings.md) object.

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
PATCH /me/settings/itemInsights
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userInsightsSettings](../resources/userinsightssettings.md) object.

The following table shows the properties that are required when you update the [userInsightsSettings](../resources/userinsightssettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isEnabled|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userinsightssettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/settings/itemInsights
Content-Type: application/json
Content-length: 89

{
  "@odata.type": "#microsoft.graph.userInsightsSettings",
  "isEnabled": "Boolean"
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
  "@odata.type": "#microsoft.graph.userInsightsSettings",
  "id": "9ea0e84d-e84d-9ea0-4de8-a09e4de8a09e",
  "isEnabled": "Boolean"
}
```

