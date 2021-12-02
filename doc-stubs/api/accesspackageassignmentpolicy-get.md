---
title: "Get accessPackageAssignmentPolicy"
description: "Read the properties and relationships of an accessPackageAssignmentPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get accessPackageAssignmentPolicy
Namespace: microsoft.graph



Read the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.

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
GET /identityGovernance/entitlementManagement/assignmentPolicies/{accessPackageAssignmentPolicyId}
GET /identityGovernance/entitlementManagement/assignments/{accessPackageAssignmentId}/assignmentPolicy
GET /identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/assignmentPolicies/{accessPackageAssignmentPolicyId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies/{accessPackageAssignmentPolicyId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageAssignmentPolicy",
    "id": "87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
    "displayName": "String",
    "description": "String",
    "allowedTargetScope": "String",
    "specificAllowedTargets": [
      {
        "@odata.type": "microsoft.graph.singleUser"
      }
    ],
    "expiration": {
      "@odata.type": "microsoft.graph.expirationPattern"
    },
    "requestorSettings": {
      "@odata.type": "microsoft.graph.accessPackageAssignmentRequestorSettings"
    },
    "requestApprovalSettings": {
      "@odata.type": "microsoft.graph.accessPackageAssignmentApprovalSettings"
    },
    "reviewSettings": {
      "@odata.type": "microsoft.graph.accessPackageAssignmentReviewSettings"
    },
    "createdDateTime": "String (timestamp)",
    "modifiedDateTime": "String (timestamp)"
  }
}
```

