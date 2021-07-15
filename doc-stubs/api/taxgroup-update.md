---
title: "Update taxGroup"
description: "Update the properties of a taxGroup object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update taxGroup
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [taxGroup](../resources/taxgroup.md) object.

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
PATCH /financials/companies/{companyId}/taxGroups/{taxGroupId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [taxGroup](../resources/taxgroup.md) object.

The following table shows the properties that are required when you update the [taxGroup](../resources/taxgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|taxType|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [taxGroup](../resources/taxgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_taxgroup"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/taxGroups/{taxGroupId}
Content-Type: application/json
Content-length: 123

{
  "@odata.type": "#microsoft.graph.taxGroup",
  "code": "String",
  "displayName": "String",
  "taxType": "String"
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
  "@odata.type": "#microsoft.graph.taxGroup",
  "id": "253b9b6a-9b6a-253b-6a9b-3b256a9b3b25",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "taxType": "String"
}
```

