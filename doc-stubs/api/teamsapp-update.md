---
title: "Update teamsApp"
description: "Update the properties of a teamsApp object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update teamsApp
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [teamsApp](../resources/teamsapp.md) object.

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
PATCH /appCatalogs/teamsApps/{teamsAppId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|externalId|String|**TODO: Add Description** Optional.|
|displayName|String|**TODO: Add Description** Optional.|
|distributionMethod|teamsAppDistributionMethod|**TODO: Add Description**. The possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`. Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [teamsApp](../resources/teamsapp.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}
Content-Type: application/json
Content-length: 140

{
  "@odata.type": "#microsoft.graph.teamsApp",
  "externalId": "String",
  "displayName": "String",
  "distributionMethod": "String"
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
  "@odata.type": "#microsoft.graph.teamsApp",
  "id": "28bb562b-562b-28bb-2b56-bb282b56bb28",
  "externalId": "String",
  "displayName": "String",
  "distributionMethod": "String"
}
```

