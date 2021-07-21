---
title: "Update onPremisesAgentGroup"
description: "Update the properties of an onPremisesAgentGroup object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update onPremisesAgentGroup
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.

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
PATCH /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agentGroups/{onPremisesAgentGroupId}
PATCH /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agentGroups/{onPremisesAgentGroupId}/agents/{onPremisesAgentId}/agentGroups/{onPremisesAgentGroupId}
PATCH /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agentGroups/{onPremisesAgentGroupId}/publishedResources/{publishedResourceId}/agentGroups/{onPremisesAgentGroupId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.

The following table shows the properties that are required when you update the [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|
|publishingType|onPremisesPublishingType|**TODO: Add Description**. Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_onpremisesagentgroup"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/agentGroups/{onPremisesAgentGroupId}
Content-Type: application/json
Content-length: 148

{
  "@odata.type": "#microsoft.graph.onPremisesAgentGroup",
  "displayName": "String",
  "isDefault": "Boolean",
  "publishingType": "String"
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
  "@odata.type": "#microsoft.graph.onPremisesAgentGroup",
  "id": "85fcefb3-efb3-85fc-b3ef-fc85b3effc85",
  "displayName": "String",
  "isDefault": "Boolean",
  "publishingType": "String"
}
```

