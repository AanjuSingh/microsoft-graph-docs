---
title: "Update windows10XSCEPCertificateProfile"
description: "Update the properties of a windows10XSCEPCertificateProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update windows10XSCEPCertificateProfile
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [windows10XSCEPCertificateProfile](../resources/windows10xscepcertificateprofile.md) object.

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
PATCH ** Entity URI for microsoft.graph.windows10XSCEPCertificateProfile not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windows10XSCEPCertificateProfile](../resources/windows10xscepcertificateprofile.md) object.

The following table shows the properties that are required when you update the [windows10XSCEPCertificateProfile](../resources/windows10xscepcertificateprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset|DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/devicemanagementresourceaccessprofilebase.md)|
|description|String|Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/devicemanagementresourceaccessprofilebase.md)|
|displayName|String|Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|String collection|Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/devicemanagementresourceaccessprofilebase.md)|
|version|Int32|Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/devicemanagementresourceaccessprofilebase.md)|
|certificateStore|certificateStore|Target store certificate. Possible values are: `user`, `machine`.|
|certificateValidityPeriodScale|certificateValidityPeriodScale|Scale for the Certificate Validity Period. Possible values are: `days`, `months`, `years`.|
|certificateValidityPeriodValue|Int32|Value for the Certificate Validity Period|
|extendedKeyUsages|[extendedKeyUsage](../resources/extendedkeyusage.md) collection|Extended Key Usage (EKU) settings.|
|hashAlgorithm|hashAlgorithms collection|SCEP Hash Algorithm. Possible values are: `sha1`, `sha2`.|
|keySize|keySize|SCEP Key Size. Possible values are: `size1024`, `size2048`, `size4096`.|
|keyStorageProvider|keyStorageProviderOption|Key Storage Provider (KSP). Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|keyUsage|keyUsages|SCEP Key Usage. Possible values are: `keyEncipherment`, `digitalSignature`.|
|renewalThresholdPercentage|Int32|Certificate renewal threshold percentage|
|rootCertificateId|Guid|Trusted Root Certificate ID|
|scepServerUrls|String collection|SCEP Server Url(s).|
|subjectAlternativeNameFormats|[windows10XCustomSubjectAlternativeName](../resources/windows10xcustomsubjectalternativename.md) collection|Custom AAD Attributes.|
|subjectNameFormatString|String|Custom format to use with SubjectNameFormat = Custom. Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US|



## Response

If successful, this method returns a `200 OK` response code and an updated [windows10XSCEPCertificateProfile](../resources/windows10xscepcertificateprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_windows10xscepcertificateprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Entity URI for microsoft.graph.windows10XSCEPCertificateProfile not found
Content-Type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
  "creationDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "Integer",
  "certificateStore": "String",
  "certificateValidityPeriodScale": "String",
  "certificateValidityPeriodValue": "Integer",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage"
    }
  ],
  "hashAlgorithm": [
    "String"
  ],
  "keySize": "String",
  "keyStorageProvider": "String",
  "keyUsage": "String",
  "renewalThresholdPercentage": "Integer",
  "rootCertificateId": "Guid",
  "scepServerUrls": [
    "String"
  ],
  "subjectAlternativeNameFormats": [
    {
      "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName"
    }
  ],
  "subjectNameFormatString": "String"
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
  "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
  "id": "d23be586-e586-d23b-86e5-3bd286e53bd2",
  "creationDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "Integer",
  "certificateStore": "String",
  "certificateValidityPeriodScale": "String",
  "certificateValidityPeriodValue": "Integer",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage"
    }
  ],
  "hashAlgorithm": [
    "String"
  ],
  "keySize": "String",
  "keyStorageProvider": "String",
  "keyUsage": "String",
  "renewalThresholdPercentage": "Integer",
  "rootCertificateId": "Guid",
  "scepServerUrls": [
    "String"
  ],
  "subjectAlternativeNameFormats": [
    {
      "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName"
    }
  ],
  "subjectNameFormatString": "String"
}
```

