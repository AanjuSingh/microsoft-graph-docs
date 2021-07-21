---
title: "Update vppToken"
description: "Update the properties of a vppToken object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update vppToken
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [vppToken](../resources/vpptoken.md) object.

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
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [vppToken](../resources/vpptoken.md) object.

The following table shows the properties that are required when you update the [vppToken](../resources/vpptoken.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appleId|String|The apple Id associated with the given Apple Volume Purchase Program Token.|
|automaticallyUpdateApps|Boolean|Whether or not apps for the VPP token will be automatically updated.|
|claimTokenManagementFromExternalMdm|Boolean|Admin consent to allow claiming token management from external MDM.|
|countryOrRegion|String|Whether or not apps for the VPP token will be automatically updated.|
|dataSharingConsentGranted|Boolean|Consent granted for data sharing with the Apple Volume Purchase Program.|
|displayName|String|An admin specified token friendly name.|
|expirationDateTime|DateTimeOffset|The expiration date time of the Apple Volume Purchase Program Token.|
|lastModifiedDateTime|DateTimeOffset|Last modification date time associated with the Apple Volume Purchase Program Token.|
|lastSyncDateTime|DateTimeOffset|The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.|
|lastSyncStatus|vppTokenSyncStatus|Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token. Possible values are: `none`, `inProgress`, `completed`, `failed`. Possible values are: `none`, `inProgress`, `completed`, `failed`.|
|locationName|String|Token location returned from Apple VPP.|
|organizationName|String|The organization associated with the Apple Volume Purchase Program Token|
|roleScopeTagIds|String collection|Role Scope Tags IDs assigned to this entity.|
|state|vppTokenState|Current state of the Apple Volume Purchase Program Token. Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`, `duplicateLocationId`.|
|token|String|The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.|
|tokenActionResults|[vppTokenActionResult](../resources/vpptokenactionresult.md) collection|The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.|
|vppTokenAccountType|vppTokenAccountType|The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. Possible values are: `business`, `education`. Possible values are: `business`, `education`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/vpptoken.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_vpptoken"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-Type: application/json
Content-length: 688

{
  "@odata.type": "#microsoft.graph.vppToken",
  "appleId": "String",
  "automaticallyUpdateApps": "Boolean",
  "claimTokenManagementFromExternalMdm": "Boolean",
  "countryOrRegion": "String",
  "dataSharingConsentGranted": "Boolean",
  "displayName": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "lastSyncStatus": "String",
  "locationName": "String",
  "organizationName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "state": "String",
  "token": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult"
    }
  ],
  "vppTokenAccountType": "String"
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
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "b94ea16d-a16d-b94e-6da1-4eb96da14eb9",
  "appleId": "String",
  "automaticallyUpdateApps": "Boolean",
  "claimTokenManagementFromExternalMdm": "Boolean",
  "countryOrRegion": "String",
  "dataSharingConsentGranted": "Boolean",
  "displayName": "String",
  "expirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "lastSyncStatus": "String",
  "locationName": "String",
  "organizationName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "state": "String",
  "token": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult"
    }
  ],
  "vppTokenAccountType": "String"
}
```

