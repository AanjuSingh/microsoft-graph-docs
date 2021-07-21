---
title: "Create governanceRoleSetting"
description: "Create a new governanceRoleSetting object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create governanceRoleSetting
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new governanceRoleSetting object.

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
POST /governanceRoleDefinitions/{governanceRoleDefinitionsId}/roleSetting
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [governanceRoleSetting](../resources/governancerolesetting.md) object.

The following table shows the properties that are required when you create the [governanceRoleSetting](../resources/governancerolesetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|
|lastUpdatedBy|String|**TODO: Add Description**|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_governancerolesetting_from_governancerolesettings"
}
-->
``` http
POST https://graph.microsoft.com/beta/governanceRoleDefinitions/{governanceRoleDefinitionsId}/roleSetting
Content-Type: application/json
Content-length: 670

{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "adminEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "adminMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "isDefault": "Boolean",
  "lastUpdatedBy": "String",
  "lastUpdatedDateTime": "String (timestamp)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "userEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "userMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "id": "6151f4b3-f4b3-6151-b3f4-5161b3f45161",
  "adminEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "adminMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "isDefault": "Boolean",
  "lastUpdatedBy": "String",
  "lastUpdatedDateTime": "String (timestamp)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "userEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "userMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ]
}
```

