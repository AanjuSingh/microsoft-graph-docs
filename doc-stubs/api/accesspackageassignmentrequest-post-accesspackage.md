---
title: "Add accessPackage"
description: "Add accessPackage by posting to the accessPackage collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add accessPackage
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add accessPackage by posting to the accessPackage collection.

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
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}/accessPackage/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackage](../resources/accesspackage.md) object.

The following table shows the properties that are required when you create the [accessPackage](../resources/accesspackage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|catalogId|String|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isHidden|Boolean|**TODO: Add Description**|
|isRoleScopesVisible|Boolean|**TODO: Add Description**|
|modifiedBy|String|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and an [accessPackage](../resources/accesspackage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackage_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}/accessPackage/$ref
Content-Type: application/json
Content-length: 253

{
  "@odata.type": "#microsoft.graph.accessPackage",
  "catalogId": "String",
  "createdBy": "String",
  "description": "String",
  "displayName": "String",
  "isHidden": "Boolean",
  "isRoleScopesVisible": "Boolean",
  "modifiedBy": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessPackage",
  "id": "bdbf1b80-1b80-bdbf-801b-bfbd801bbfbd",
  "catalogId": "String",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "isHidden": "Boolean",
  "isRoleScopesVisible": "Boolean",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

