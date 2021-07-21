---
title: "Get depEnrollmentProfile"
description: "Read the properties and relationships of a depEnrollmentProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get depEnrollmentProfile
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [depEnrollmentProfile](../resources/depenrollmentprofile.md) object.

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
GET /depEnrollmentProfile
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

If successful, this method returns a `200 OK` response code and a [depEnrollmentProfile](../resources/depenrollmentprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_depenrollmentprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/depEnrollmentProfile
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.depEnrollmentProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.depEnrollmentProfile",
    "id": "54e8529e-529e-54e8-9e52-e8549e52e854",
    "configurationEndpointUrl": "String",
    "description": "String",
    "displayName": "String",
    "enableAuthenticationViaCompanyPortal": "Boolean",
    "requireCompanyPortalOnSetupAssistantEnrolledDevices": "Boolean",
    "requiresUserAuthentication": "Boolean",
    "appleIdDisabled": "Boolean",
    "applePayDisabled": "Boolean",
    "awaitDeviceConfiguredConfirmation": "Boolean",
    "diagnosticsDisabled": "Boolean",
    "enableSharedIPad": "Boolean",
    "isDefault": "Boolean",
    "isMandatory": "Boolean",
    "iTunesPairingMode": "String",
    "locationDisabled": "Boolean",
    "macOSFileVaultDisabled": "Boolean",
    "macOSRegistrationDisabled": "Boolean",
    "managementCertificates": [
      {
        "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
      }
    ],
    "passCodeDisabled": "Boolean",
    "profileRemovalDisabled": "Boolean",
    "restoreBlocked": "Boolean",
    "restoreFromAndroidDisabled": "Boolean",
    "sharedIPadMaximumUserCount": "Integer",
    "siriDisabled": "Boolean",
    "supervisedModeEnabled": "Boolean",
    "supportDepartment": "String",
    "supportPhoneNumber": "String",
    "termsAndConditionsDisabled": "Boolean",
    "touchIdDisabled": "Boolean",
    "zoomDisabled": "Boolean"
  }
}
```

