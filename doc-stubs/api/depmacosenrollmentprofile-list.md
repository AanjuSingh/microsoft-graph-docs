---
title: "List depMacOSEnrollmentProfiles"
description: "Get a list of the depMacOSEnrollmentProfile objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List depMacOSEnrollmentProfiles
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.depMacOSEnrollmentProfile not found
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

If successful, this method returns a `200 OK` response code and a collection of [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_depmacosenrollmentprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.depMacOSEnrollmentProfile not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.depMacOSEnrollmentProfile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
      "id": "23f4e4e3-e4e3-23f4-e3e4-f423e3e4f423",
      "configurationEndpointUrl": "String",
      "description": "String",
      "displayName": "String",
      "enableAuthenticationViaCompanyPortal": "Boolean",
      "requireCompanyPortalOnSetupAssistantEnrolledDevices": "Boolean",
      "requiresUserAuthentication": "Boolean",
      "appleIdDisabled": "Boolean",
      "applePayDisabled": "Boolean",
      "configurationWebUrl": "Boolean",
      "deviceNameTemplate": "String",
      "diagnosticsDisabled": "Boolean",
      "displayToneSetupDisabled": "Boolean",
      "isDefault": "Boolean",
      "isMandatory": "Boolean",
      "locationDisabled": "Boolean",
      "privacyPaneDisabled": "Boolean",
      "profileRemovalDisabled": "Boolean",
      "restoreBlocked": "Boolean",
      "screenTimeScreenDisabled": "Boolean",
      "siriDisabled": "Boolean",
      "supervisedModeEnabled": "Boolean",
      "supportDepartment": "String",
      "supportPhoneNumber": "String",
      "termsAndConditionsDisabled": "Boolean",
      "touchIdDisabled": "Boolean",
      "accessibilityScreenDisabled": "Boolean",
      "chooseYourLockScreenDisabled": "Boolean",
      "fileVaultDisabled": "Boolean",
      "iCloudDiagnosticsDisabled": "Boolean",
      "iCloudStorageDisabled": "Boolean",
      "passCodeDisabled": "Boolean",
      "registrationDisabled": "Boolean",
      "zoomDisabled": "Boolean"
    }
  ]
}
```

