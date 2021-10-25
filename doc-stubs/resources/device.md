---
title: "device resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# device resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List devices](../api/device-list.md)|[device](../resources/device.md) collection|Get a list of the [device](../resources/device.md) objects and their properties.|
|[Create device](../api/device-post-devices.md)|[device](../resources/device.md)|Create a new [device](../resources/device.md) object.|
|[Get device](../api/device-get.md)|[device](../resources/device.md)|Read the properties and relationships of a [device](../resources/device.md) object.|
|[Update device](../api/device-update.md)|[device](../resources/device.md)|Update the properties of a [device](../resources/device.md) object.|
|[Delete device](../api/device-delete.md)|None|Deletes a [device](../resources/device.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean|**TODO: Add Description**|
|alternativeSecurityIds|[alternativeSecurityId](../resources/alternativesecurityid.md) collection|**TODO: Add Description**|
|approximateLastSignInDateTime|DateTimeOffset|**TODO: Add Description**|
|capabilities|deviceCapabilities collection|**TODO: Add Description**|
|complianceExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|compliantApplications|[compliantApplication](../resources/compliantapplication.md) collection|**TODO: Add Description**|
|compliantApplicationsManagementAppId|String|**TODO: Add Description**|
|customSecurityAttributes|[customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md).|
|deviceCategory|String|**TODO: Add Description**|
|deviceId|String|**TODO: Add Description**|
|deviceKeys|[deviceKey](../resources/devicekey.md) collection|**TODO: Add Description**|
|deviceMetadata|String|**TODO: Add Description**|
|deviceOwnership|String|**TODO: Add Description**|
|deviceSystemMetadata|[keyValue](../resources/keyvalue.md)|**TODO: Add Description**|
|deviceVersion|Int32|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|domainName|String|**TODO: Add Description**|
|enrollmentProfileName|String|**TODO: Add Description**|
|enrollmentType|String|**TODO: Add Description**|
|exchangeActiveSyncIds|String collection|**TODO: Add Description**|
|extensionAttributes|[onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md)|**TODO: Add Description**|
|hostnames|String collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|isCompliant|Boolean|**TODO: Add Description**|
|isManaged|Boolean|**TODO: Add Description**|
|isManagementRestricted|Boolean|**TODO: Add Description**|
|isRooted|Boolean|**TODO: Add Description**|
|kind|String|**TODO: Add Description**|
|localCredentials|String|**TODO: Add Description**|
|managementType|String|**TODO: Add Description**|
|manufacturer|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|operatingSystem|String|**TODO: Add Description**|
|operatingSystemVersion|String|**TODO: Add Description**|
|organizationalUnit|String|**TODO: Add Description**|
|physicalIds|String collection|**TODO: Add Description**|
|platform|String|**TODO: Add Description**|
|profileType|String|**TODO: Add Description**|
|registrationDateTime|DateTimeOffset|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|systemLabels|String collection|**TODO: Add Description**|
|trustType|String|**TODO: Add Description**|
|userCertificate|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|commands|[command](../resources/command.md) collection|**TODO: Add Description**|
|extensions|[extension](../resources/extension.md) collection|**TODO: Add Description**|
|memberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|registeredOwners|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|registeredUsers|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|usageRights|[usageRight](../resources/usageright.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.device",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "accountEnabled": "Boolean",
  "alternativeSecurityIds": [
    {
      "@odata.type": "microsoft.graph.alternativeSecurityId"
    }
  ],
  "approximateLastSignInDateTime": "String (timestamp)",
  "capabilities": [
    "String"
  ],
  "complianceExpirationDateTime": "String (timestamp)",
  "compliantApplications": [
    {
      "@odata.type": "microsoft.graph.compliantApplication"
    }
  ],
  "compliantApplicationsManagementAppId": "String",
  "customSecurityAttributes": {
    "@odata.type": "microsoft.graph.customSecurityAttributeValue"
  },
  "deviceCategory": "String",
  "deviceId": "String",
  "deviceKeys": [
    {
      "@odata.type": "microsoft.graph.deviceKey"
    }
  ],
  "deviceMetadata": "String",
  "deviceOwnership": "String",
  "deviceSystemMetadata": {
    "@odata.type": "microsoft.graph.keyValue"
  },
  "deviceVersion": "Integer",
  "displayName": "String",
  "domainName": "String",
  "enrollmentProfileName": "String",
  "enrollmentType": "String",
  "exchangeActiveSyncIds": [
    "String"
  ],
  "extensionAttributes": {
    "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
  },
  "hostnames": [
    "String"
  ],
  "isCompliant": "Boolean",
  "isManaged": "Boolean",
  "isManagementRestricted": "Boolean",
  "isRooted": "Boolean",
  "kind": "String",
  "localCredentials": "String",
  "managementType": "String",
  "manufacturer": "String",
  "model": "String",
  "name": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": "Boolean",
  "operatingSystem": "String",
  "operatingSystemVersion": "String",
  "organizationalUnit": "String",
  "physicalIds": [
    "String"
  ],
  "platform": "String",
  "profileType": "String",
  "registrationDateTime": "String (timestamp)",
  "status": "String",
  "systemLabels": [
    "String"
  ],
  "trustType": "String",
  "userCertificate": "String"
}
```

