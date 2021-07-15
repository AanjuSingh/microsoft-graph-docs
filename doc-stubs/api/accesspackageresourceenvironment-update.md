---
title: "Update accessPackageResourceEnvironment"
description: "Update the properties of an accessPackageResourceEnvironment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessPackageResourceEnvironment
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.

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
PATCH /identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}/accessPackage/accessPackageCatalog/accessPackageResourceRoles/{accessPackageResourceRoleId}/accessPackageResource/accessPackageResourceEnvironment
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.

The following table shows the properties that are required when you update the [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|connectionInfo|[connectionInfo](../resources/connectioninfo.md)|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isDefaultEnvironment|Boolean|**TODO: Add Description**|
|modifiedBy|String|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|originId|String|**TODO: Add Description**|
|originSystem|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackageresourceenvironment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
Content-Type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.accessPackageResourceEnvironment",
  "connectionInfo": {
    "@odata.type": "microsoft.graph.connectionInfo"
  },
  "createdBy": "String",
  "description": "String",
  "displayName": "String",
  "isDefaultEnvironment": "Boolean",
  "modifiedBy": "String",
  "originId": "String",
  "originSystem": "String"
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
  "@odata.type": "#microsoft.graph.accessPackageResourceEnvironment",
  "id": "35843e20-3e20-3584-203e-8435203e8435",
  "connectionInfo": {
    "@odata.type": "microsoft.graph.connectionInfo"
  },
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "isDefaultEnvironment": "Boolean",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "originId": "String",
  "originSystem": "String"
}
```

