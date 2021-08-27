---
title: "Create entitlementManagementSettings"
description: "Create a new entitlementManagementSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create entitlementManagementSettings
Namespace: microsoft.graph



Create a new entitlementManagementSettings object.

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
POST /entitlementManagement/settings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.

The following table shows the properties that are required when you create the [entitlementManagementSettings](../resources/entitlementmanagementsettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|externalUserLifecycleAction|accessPackageExternalUserLifecycleAction|**TODO: Add Description**. The possible values are: `none`, `blockSignIn`, `blockSignInAndDelete`, `unknownFutureValue`.|
|durationUntilExternalUserDeletedAfterBlocked|Duration|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_entitlementmanagementsettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/entitlementManagement/settings
Content-Type: application/json
Content-length: 214

{
  "@odata.type": "#Microsoft.IGAELM.EC.FrontEnd.ExternalModel.entitlementManagementSettings",
  "externalUserLifecycleAction": "String",
  "durationUntilExternalUserDeletedAfterBlocked": "String (duration)"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.IGAELM.EC.FrontEnd.ExternalModel.entitlementManagementSettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.IGAELM.EC.FrontEnd.ExternalModel.entitlementManagementSettings",
  "id": "a5df80e0-80e0-a5df-e080-dfa5e080dfa5",
  "externalUserLifecycleAction": "String",
  "durationUntilExternalUserDeletedAfterBlocked": "String (duration)"
}
```

