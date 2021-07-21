---
title: "Create managedDeviceCertificateState"
description: "Create a new managedDeviceCertificateState object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managedDeviceCertificateState
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new managedDeviceCertificateState object.

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
POST ** Collection URI for microsoft.graph.managedDeviceCertificateState not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) object.

The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|certificateEnhancedKeyUsage|String|Extended key usage|
|certificateErrorCode|Int32|Error code|
|certificateExpirationDateTime|DateTimeOffset|Certificate expiry date|
|certificateIssuanceDateTime|DateTimeOffset|Issuance date|
|certificateIssuanceState|certificateIssuanceStates|Issuance State. Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.|
|certificateIssuer|String|Issuer|
|certificateKeyLength|Int32|Key length|
|certificateKeyStorageProvider|keyStorageProviderOption|Key Storage Provider. Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|certificateKeyUsage|keyUsages|Key usage. Possible values are: `keyEncipherment`, `digitalSignature`.|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|Last certificate issuance state change|
|certificateProfileDisplayName|String|Certificate profile display name|
|certificateRevokeStatus|certificateRevocationStatus|Revoke status. Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateSerialNumber|String|Serial number|
|certificateSubjectAlternativeNameFormat|subjectAlternativeNameType|Subject alternative name format. Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.|
|certificateSubjectAlternativeNameFormatString|String|Subject alternative name format string for custom formats|
|certificateSubjectNameFormat|subjectNameFormat|Subject name format. Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateSubjectNameFormatString|String|Subject name format string for custom subject name formats|
|certificateThumbprint|String|Thumbprint|
|certificateValidityPeriod|Int32|Validity period|
|certificateValidityPeriodUnits|certificateValidityPeriodScale|Validity period units. Possible values are: `days`, `months`, `years`.|
|deviceDisplayName|String|Device display name|
|devicePlatform|devicePlatformType|Device platform. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`, `androidAOSP`.|
|lastCertificateStateChangeDateTime|DateTimeOffset|Last certificate issuance state change|
|userDisplayName|String|User display name|



## Response

If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_manageddevicecertificatestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.managedDeviceCertificateState not found
Content-Type: application/json
Content-length: 1162

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "certificateEnhancedKeyUsage": "String",
  "certificateErrorCode": "Integer",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateIssuanceDateTime": "String (timestamp)",
  "certificateIssuanceState": "String",
  "certificateIssuer": "String",
  "certificateKeyLength": "Integer",
  "certificateKeyStorageProvider": "String",
  "certificateKeyUsage": "String",
  "certificateLastIssuanceStateChangedDateTime": "String (timestamp)",
  "certificateProfileDisplayName": "String",
  "certificateRevokeStatus": "String",
  "certificateSerialNumber": "String",
  "certificateSubjectAlternativeNameFormat": "String",
  "certificateSubjectAlternativeNameFormatString": "String",
  "certificateSubjectNameFormat": "String",
  "certificateSubjectNameFormatString": "String",
  "certificateThumbprint": "String",
  "certificateValidityPeriod": "Integer",
  "certificateValidityPeriodUnits": "String",
  "deviceDisplayName": "String",
  "devicePlatform": "String",
  "lastCertificateStateChangeDateTime": "String (timestamp)",
  "userDisplayName": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedDeviceCertificateState"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "0d89b793-b793-0d89-93b7-890d93b7890d",
  "certificateEnhancedKeyUsage": "String",
  "certificateErrorCode": "Integer",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateIssuanceDateTime": "String (timestamp)",
  "certificateIssuanceState": "String",
  "certificateIssuer": "String",
  "certificateKeyLength": "Integer",
  "certificateKeyStorageProvider": "String",
  "certificateKeyUsage": "String",
  "certificateLastIssuanceStateChangedDateTime": "String (timestamp)",
  "certificateProfileDisplayName": "String",
  "certificateRevokeStatus": "String",
  "certificateSerialNumber": "String",
  "certificateSubjectAlternativeNameFormat": "String",
  "certificateSubjectAlternativeNameFormatString": "String",
  "certificateSubjectNameFormat": "String",
  "certificateSubjectNameFormatString": "String",
  "certificateThumbprint": "String",
  "certificateValidityPeriod": "Integer",
  "certificateValidityPeriodUnits": "String",
  "deviceDisplayName": "String",
  "devicePlatform": "String",
  "lastCertificateStateChangeDateTime": "String (timestamp)",
  "userDisplayName": "String"
}
```

