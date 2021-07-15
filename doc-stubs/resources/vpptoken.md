---
title: "vppToken resource type"
description: "You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education. This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune. You can then synchronize your volume purchase information with Intune and track your volume-purchased app use. You can upload multiple Apple VPP Business or Education tokens."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# vppToken resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education. This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune. You can then synchronize your volume purchase information with Intune and track your volume-purchased app use. You can upload multiple Apple VPP Business or Education tokens.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List vppTokens](../api/vpptoken-list.md)|[vppToken](../resources/vpptoken.md) collection|Get a list of the [vppToken](../resources/vpptoken.md) objects and their properties.|
|[Create vppToken](../api/vpptoken-create.md)|[vppToken](../resources/vpptoken.md)|Create a new [vppToken](../resources/vpptoken.md) object.|
|[Get vppToken](../api/vpptoken-get.md)|[vppToken](../resources/vpptoken.md)|Read the properties and relationships of a [vppToken](../resources/vpptoken.md) object.|
|[Update vppToken](../api/vpptoken-update.md)|[vppToken](../resources/vpptoken.md)|Update the properties of a [vppToken](../resources/vpptoken.md) object.|
|[Delete vppToken](../api/vpptoken-delete.md)|None|Deletes a [vppToken](../resources/vpptoken.md) object.|
|[revokeLicenses](../api/vpptoken-revokelicenses.md)|None|Revoke licenses associated with a specific appleVolumePurchaseProgramToken|
|[syncLicenses](../api/vpptoken-synclicenses.md)|[vppToken](../resources/vpptoken.md)|Syncs licenses associated with a specific appleVolumePurchaseProgramToken|
|[syncLicenseCounts](../api/vpptoken-synclicensecounts.md)|None|**TODO: Add Description**|
|[getLicensesForApp](../api/vpptoken-getlicensesforapp.md)|[vppTokenLicenseSummary](../resources/vpptokenlicensesummary.md) collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleId|String|The apple Id associated with the given Apple Volume Purchase Program Token.|
|automaticallyUpdateApps|Boolean|Whether or not apps for the VPP token will be automatically updated.|
|claimTokenManagementFromExternalMdm|Boolean|Admin consent to allow claiming token management from external MDM.|
|countryOrRegion|String|Whether or not apps for the VPP token will be automatically updated.|
|dataSharingConsentGranted|Boolean|Consent granted for data sharing with the Apple Volume Purchase Program.|
|displayName|String|An admin specified token friendly name.|
|expirationDateTime|DateTimeOffset|The expiration date time of the Apple Volume Purchase Program Token.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
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

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
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

