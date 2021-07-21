---
title: "Update cloudPcProvisioningPolicyAssignment"
description: "Update the properties of a cloudPcProvisioningPolicyAssignment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update cloudPcProvisioningPolicyAssignment
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.

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
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{cloudPcProvisioningPolicyId}/assignments/{cloudPcProvisioningPolicyAssignmentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.

The following table shows the properties that are required when you update the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|target|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_cloudpcprovisioningpolicyassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{cloudPcProvisioningPolicyId}/assignments/{cloudPcProvisioningPolicyAssignmentId}
Content-Type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementAssignmentTarget"
  }
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
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "id": "ab810c64-0c64-ab81-640c-81ab640c81ab",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementAssignmentTarget"
  }
}
```

