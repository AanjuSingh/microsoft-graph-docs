---
title: "user: getLoggedOnManagedDevices"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# user: getLoggedOnManagedDevices
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

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
GET /me/getLoggedOnManagedDevices
GET /users/{usersId}/getLoggedOnManagedDevices
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [managedDevice](../resources/manageddevice.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_getloggedonmanageddevices"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/getLoggedOnManagedDevices
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedDevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "String (identifier)",
      "cloudPcRemoteActionResults": [
        {
          "@odata.type": "microsoft.graph.cloudPcRemoteActionResult"
        }
      ],
      "aadRegistered": "Boolean",
      "activationLockBypassCode": "String",
      "androidSecurityPatchLevel": "String",
      "autopilotEnrolled": "Boolean",
      "azureActiveDirectoryDeviceId": "String",
      "azureADDeviceId": "String",
      "azureADRegistered": "Boolean",
      "chassisType": "String",
      "chromeOSDeviceInfo": [
        {
          "@odata.type": "microsoft.graph.chromeOSDeviceProperty"
        }
      ],
      "complianceGracePeriodExpirationDateTime": "String (timestamp)",
      "complianceState": "String",
      "configurationManagerClientEnabledFeatures": {
        "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
      },
      "configurationManagerClientHealthState": {
        "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
      },
      "configurationManagerClientInformation": {
        "@odata.type": "microsoft.graph.configurationManagerClientInformation"
      },
      "deviceActionResults": [
        {
          "@odata.type": "microsoft.graph.deviceActionResult"
        }
      ],
      "deviceCategoryDisplayName": "String",
      "deviceEnrollmentType": "String",
      "deviceHealthAttestationState": {
        "@odata.type": "microsoft.graph.deviceHealthAttestationState"
      },
      "deviceName": "String",
      "deviceRegistrationState": "String",
      "deviceType": "String",
      "easActivated": "Boolean",
      "easActivationDateTime": "String (timestamp)",
      "easDeviceId": "String",
      "emailAddress": "String",
      "enrolledDateTime": "String (timestamp)",
      "ethernetMacAddress": "String",
      "exchangeAccessState": "String",
      "exchangeAccessStateReason": "String",
      "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
      "freeStorageSpaceInBytes": "Integer",
      "hardwareInformation": {
        "@odata.type": "microsoft.graph.hardwareInformation"
      },
      "iccid": "String",
      "imei": "String",
      "isEncrypted": "Boolean",
      "isSupervised": "Boolean",
      "jailBroken": "String",
      "joinType": "String",
      "lastSyncDateTime": "String (timestamp)",
      "lostModeState": "String",
      "managedDeviceName": "String",
      "managedDeviceOwnerType": "String",
      "managementAgent": "String",
      "managementCertificateExpirationDate": "String (timestamp)",
      "managementFeatures": "String",
      "managementState": "String",
      "manufacturer": "String",
      "meid": "String",
      "model": "String",
      "notes": "String",
      "operatingSystem": "String",
      "osVersion": "String",
      "ownerType": "String",
      "partnerReportedThreatState": "String",
      "phoneNumber": "String",
      "physicalMemoryInBytes": "Integer",
      "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
      "processorArchitecture": "String",
      "remoteAssistanceSessionErrorDetails": "String",
      "remoteAssistanceSessionUrl": "String",
      "requireUserEnrollmentApproval": "Boolean",
      "retireAfterDateTime": "String (timestamp)",
      "roleScopeTagIds": [
        "String"
      ],
      "serialNumber": "String",
      "skuFamily": "String",
      "skuNumber": "Integer",
      "specificationVersion": "String",
      "subscriberCarrier": "String",
      "totalStorageSpaceInBytes": "Integer",
      "udid": "String",
      "userDisplayName": "String",
      "userId": "String",
      "userPrincipalName": "String",
      "usersLoggedOn": [
        {
          "@odata.type": "microsoft.graph.loggedOnUser"
        }
      ],
      "wiFiMacAddress": "String",
      "windowsActiveMalwareCount": "Integer",
      "windowsRemediatedMalwareCount": "Integer"
    }
  ]
}
```

