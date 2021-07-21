---
title: "mdmWindowsInformationProtectionPolicy resource type"
description: "Policy for Windows information protection with MDM"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mdmWindowsInformationProtectionPolicy resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Policy for Windows information protection with MDM


Inherits from [windowsInformationProtection](../resources/windowsinformationprotection.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List mdmWindowsInformationProtectionPolicies](../api/mdmwindowsinformationprotectionpolicy-list.md)|[mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md) collection|Get a list of the [mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md) objects and their properties.|
|[Create mdmWindowsInformationProtectionPolicy](../api/mdmwindowsinformationprotectionpolicy-create.md)|[mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md)|Create a new [mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md) object.|
|[Get mdmWindowsInformationProtectionPolicy](../api/mdmwindowsinformationprotectionpolicy-get.md)|[mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md)|Read the properties and relationships of a [mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md) object.|
|[Update mdmWindowsInformationProtectionPolicy](../api/mdmwindowsinformationprotectionpolicy-update.md)|[mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md)|Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md) object.|
|[Delete mdmWindowsInformationProtectionPolicy](../api/mdmwindowsinformationprotectionpolicy-delete.md)|None|Deletes a [mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md) object.|
|[assign](../api/mdmwindowsinformationprotectionpolicy-assign.md)|None|**TODO: Add Description**|
|[hasPayloadLinks](../api/mdmwindowsinformationprotectionpolicy-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection|**TODO: Add Description**|
|[List assignments](../api/mdmwindowsinformationprotectionpolicy-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignment resources from the assignments navigation property.|
|[Create targetedManagedAppPolicyAssignment](../api/mdmwindowsinformationprotectionpolicy-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Create a new targetedManagedAppPolicyAssignment object.|
|[List exemptAppLockerFiles](../api/mdmwindowsinformationprotectionpolicy-list-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFile resources from the exemptAppLockerFiles navigation property.|
|[Create windowsInformationProtectionAppLockerFile](../api/mdmwindowsinformationprotectionpolicy-post-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Create a new windowsInformationProtectionAppLockerFile object.|
|[List protectedAppLockerFiles](../api/mdmwindowsinformationprotectionpolicy-list-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFile resources from the protectedAppLockerFiles navigation property.|
|[Create windowsInformationProtectionAppLockerFile](../api/mdmwindowsinformationprotectionpolicy-post-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Create a new windowsInformationProtectionAppLockerFile object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureRightsManagementServicesAllowed|Boolean|Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|createdDateTime|DateTimeOffset|The date and time the policy was created. Inherited from [managedAppPolicy](../resources/managedapppolicy.md).|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/windowsinformationprotectiondatarecoverycertificate.md)|Specifies a recovery certificate that can be used for data recovery of encrypted files. This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|description|String|The policy's description. Inherited from [managedAppPolicy](../resources/managedapppolicy.md).|
|displayName|String|Policy display name. Inherited from [managedAppPolicy](../resources/managedapppolicy.md).|
|enforcementLevel|windowsInformationProtectionEnforcementLevel|WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md). Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
|enterpriseDomain|String|Primary enterprise domain Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|This is the comma-separated list of internal proxy server eProxiedDomains policy to force traffic t ugh these proxies Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/windowsinformationprotectioniprangecollection.md) collection|Sets the enterprise IP ranges that define the computers in the enterprise network. Data that comes from those computers will be considered part of the enterprise and protected. These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|enterpriseIPRangesAreAuthoritative|Boolean|Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets. Default is false Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|This is the list of domains that comprise the boundaries of the enterprise. Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/windowsinformationprotectionproxieddomaincollection.md) collection|Contains a list of Enterprise resource domains hosted in the cloud that need to be protected. Connections to these resources are considered enterprise data. If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80). A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|This is a list of proxy servers. Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|enterpriseProxyServersAreAuthoritative|Boolean|Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies. Default is false Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|exemptApps|[windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md) collection|Exempt applications can also access enterprise data, but the data handled by those applications are not protected. This is because some critical enterprise applications may have compatibility problems with encrypted data. Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|iconsVisible|Boolean|Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu. Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|indexingEncryptedStoresOrItemsBlocked|Boolean|This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|isAssigned|Boolean|Indicates if the policy is deployed to any inclusion groups or not. Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|lastModifiedDateTime|DateTimeOffset|Last time the policy was modified. Inherited from [managedAppPolicy](../resources/managedapppolicy.md).|
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|protectedApps|[windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md) collection|Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|protectionUnderLockConfigRequired|Boolean|Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|revokeOnUnenrollDisabled|Boolean|This policy controls whether to revoke the WIP keys when a device unenrolls from the management service. If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment. If the keys are not revoked, there will be no revoked file cleanup subsequently. Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|rightsManagementServicesTemplateId|Guid|TemplateID GUID to use for RMS encryption. The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [managedAppPolicy](../resources/managedapppolicy.md).|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md).|
|version|String|Version of the entity. Inherited from [managedAppPolicy](../resources/managedapppolicy.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Navigation property to list of security groups targeted for policy. Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Another way to input exempt apps through xml files Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Another way to input protected apps through xml files Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "baseType": "microsoft.graph.windowsInformationProtection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "azureRightsManagementServicesAllowed": "Boolean",
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
  },
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
    }
  ],
  "enterpriseIPRangesAreAuthoritative": "Boolean",
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
    }
  ],
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProxyServersAreAuthoritative": "Boolean",
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
    }
  ],
  "iconsVisible": "Boolean",
  "indexingEncryptedStoresOrItemsBlocked": "Boolean",
  "isAssigned": "Boolean",
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
    }
  ],
  "protectionUnderLockConfigRequired": "Boolean",
  "revokeOnUnenrollDisabled": "Boolean",
  "rightsManagementServicesTemplateId": "Guid",
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ]
}
```

