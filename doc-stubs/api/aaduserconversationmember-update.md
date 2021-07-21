---
title: "Update aadUserConversationMember"
description: "Update the properties of an aadUserConversationMember object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update aadUserConversationMember
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [aadUserConversationMember](../resources/aaduserconversationmember.md) object.

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
PATCH /aadUserConversationMember
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [aadUserConversationMember](../resources/aaduserconversationmember.md) object.

The following table shows the properties that are required when you update the [aadUserConversationMember](../resources/aaduserconversationmember.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [conversationMember](../resources/conversationmember.md)|
|roles|String collection|**TODO: Add Description** Inherited from [conversationMember](../resources/conversationmember.md)|
|visibleHistoryStartDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [conversationMember](../resources/conversationmember.md)|
|email|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [aadUserConversationMember](../resources/aaduserconversationmember.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_aaduserconversationmember"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/aadUserConversationMember
Content-Type: application/json
Content-length: 255

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "displayName": "String",
  "roles": [
    "String"
  ],
  "visibleHistoryStartDateTime": "String (timestamp)",
  "email": "String",
  "tenantId": "String",
  "userId": "String"
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
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "faf74d9b-4d9b-faf7-9b4d-f7fa9b4df7fa",
  "displayName": "String",
  "roles": [
    "String"
  ],
  "visibleHistoryStartDateTime": "String (timestamp)",
  "email": "String",
  "tenantId": "String",
  "userId": "String"
}
```

