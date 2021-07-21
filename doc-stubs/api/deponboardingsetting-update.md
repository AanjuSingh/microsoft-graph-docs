---
title: "Update depOnboardingSetting"
description: "Update the properties of a depOnboardingSetting object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update depOnboardingSetting
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [depOnboardingSetting](../resources/deponboardingsetting.md) object.

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
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [depOnboardingSetting](../resources/deponboardingsetting.md) object.

The following table shows the properties that are required when you update the [depOnboardingSetting](../resources/deponboardingsetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appleIdentifier|String|The Apple ID used to obtain the current token.|
|dataSharingConsentGranted|Boolean|Consent granted for data sharing with Apple Dep Service|
|lastModifiedDateTime|DateTimeOffset|When the service was onboarded.|
|lastSuccessfulSyncDateTime|DateTimeOffset|When the service last syned with Intune|
|lastSyncErrorCode|Int32|Error code reported by Apple during last dep sync.|
|lastSyncTriggeredDateTime|DateTimeOffset|When Intune last requested a sync.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|
|shareTokenWithSchoolDataSyncService|Boolean|Whether or not the Dep token sharing is enabled with the School Data Sync service.|
|syncedDeviceCount|Int32|Gets synced device count|
|tokenExpirationDateTime|DateTimeOffset|When the token will expire.|
|tokenName|String|Friendly Name for Dep Token|
|tokenType|depTokenType|Gets or sets the Dep Token Type. Possible values are: `none`, `dep`, `appleSchoolManager`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/deponboardingsetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_deponboardingsetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-Type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "String",
  "dataSharingConsentGranted": "Boolean",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "lastSyncErrorCode": "Integer",
  "lastSyncTriggeredDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "shareTokenWithSchoolDataSyncService": "Boolean",
  "syncedDeviceCount": "Integer",
  "tokenExpirationDateTime": "String (timestamp)",
  "tokenName": "String",
  "tokenType": "String"
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
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "4d1d05e3-05e3-4d1d-e305-1d4de3051d4d",
  "appleIdentifier": "String",
  "dataSharingConsentGranted": "Boolean",
  "lastModifiedDateTime": "String (timestamp)",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "lastSyncErrorCode": "Integer",
  "lastSyncTriggeredDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "shareTokenWithSchoolDataSyncService": "Boolean",
  "syncedDeviceCount": "Integer",
  "tokenExpirationDateTime": "String (timestamp)",
  "tokenName": "String",
  "tokenType": "String"
}
```

