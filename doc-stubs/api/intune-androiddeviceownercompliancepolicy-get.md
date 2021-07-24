---
title: "Get androidDeviceOwnerCompliancePolicy"
description: "Read the properties and relationships of an androidDeviceOwnerCompliancePolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get androidDeviceOwnerCompliancePolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [androidDeviceOwnerCompliancePolicy](../resources/intune-androiddeviceownercompliancepolicy.md) object.

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
GET ** Entity URI for microsoft.graph.androidDeviceOwnerCompliancePolicy not found
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

If successful, this method returns a `200 OK` response code and an [androidDeviceOwnerCompliancePolicy](../resources/intune-androiddeviceownercompliancepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_androiddeviceownercompliancepolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.graph.androidDeviceOwnerCompliancePolicy not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidDeviceOwnerCompliancePolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
    "id": "d8946935-6935-d894-3569-94d8356994d8",
    "roleScopeTagIds": [
      "String"
    ],
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "displayName": "String",
    "version": "Integer",
    "deviceThreatProtectionEnabled": "Boolean",
    "deviceThreatProtectionRequiredSecurityLevel": "String",
    "advancedThreatProtectionRequiredSecurityLevel": "String",
    "securityRequireSafetyNetAttestationBasicIntegrity": "Boolean",
    "securityRequireSafetyNetAttestationCertifiedDevice": "Boolean",
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "minAndroidSecurityPatchLevel": "String",
    "passwordRequired": "Boolean",
    "passwordMinimumLength": "Integer",
    "passwordMinimumLetterCharacters": "Integer",
    "passwordMinimumLowerCaseCharacters": "Integer",
    "passwordMinimumNonLetterCharacters": "Integer",
    "passwordMinimumNumericCharacters": "Integer",
    "passwordMinimumSymbolCharacters": "Integer",
    "passwordMinimumUpperCaseCharacters": "Integer",
    "passwordRequiredType": "String",
    "passwordMinutesOfInactivityBeforeLock": "Integer",
    "passwordExpirationDays": "Integer",
    "passwordPreviousPasswordCountToBlock": "Integer",
    "storageRequireEncryption": "Boolean",
    "securityRequireIntuneAppIntegrity": "Boolean"
  }
}
```

