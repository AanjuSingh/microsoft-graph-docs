---
title: "intuneBrandingProfile resource type"
description: "This entity contains data which is used in customizing the tenant level appearance of the Company Portal applications as well as the end user web portal."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# intuneBrandingProfile resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

This entity contains data which is used in customizing the tenant level appearance of the Company Portal applications as well as the end user web portal.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List intuneBrandingProfiles](../api/intunebrandingprofile-list.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md) collection|Get a list of the [intuneBrandingProfile](../resources/intunebrandingprofile.md) objects and their properties.|
|[Create intuneBrandingProfile](../api/intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md)|Create a new [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.|
|[Get intuneBrandingProfile](../api/intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md)|Read the properties and relationships of an [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.|
|[Update intuneBrandingProfile](../api/intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md)|Update the properties of an [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.|
|[Delete intuneBrandingProfile](../api/intunebrandingprofile-delete.md)|None|Deletes an [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.|
|[assign](../api/intunebrandingprofile-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/intunebrandingprofile-list-assignments.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) collection|Get the intuneBrandingProfileAssignment resources from the assignments navigation property.|
|[Create intuneBrandingProfileAssignment](../api/intunebrandingprofile-post-assignments.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Create a new intuneBrandingProfileAssignment object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|companyPortalBlockedActions|[companyPortalBlockedAction](../resources/companyportalblockedaction.md) collection|Collection of blocked actions on the company portal as per platform and device ownership types.|
|contactITEmailAddress|String|E-mail address of the person/organization responsible for IT support|
|contactITName|String|Name of the person/organization responsible for IT support|
|contactITNotes|String|Text comments regarding the person/organization responsible for IT support|
|contactITPhoneNumber|String|Phone number of the person/organization responsible for IT support|
|createdDateTime|DateTimeOffset|Time when the BrandingProfile was created|
|customCanSeePrivacyMessage|String|Text comments regarding what the admin has access to on the device|
|customCantSeePrivacyMessage|String|Text comments regarding what the admin doesn't have access to on the device|
|customPrivacyMessage|String|Text comments regarding what the admin doesn't have access to on the device|
|disableClientTelemetry|Boolean|Applies to telemetry sent from all clients to the Intune service. When disabled, all proactive troubleshooting and issue warnings within the client are turned off, and telemetry settings appear inactive or hidden to the device user.|
|displayName|String|Company/organization name that is displayed to end users|
|enrollmentAvailability|enrollmentAvailabilityOptions|Customized device enrollment flow displayed to the end user . Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|isDefaultProfile|Boolean|Boolean that represents whether the profile is used as default or not|
|isFactoryResetDisabled|Boolean|Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.|
|isRemoveDeviceDisabled|Boolean|Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.|
|landingPageCustomizedImage|[mimeContent](../resources/mimecontent.md)|Customized image displayed in Company Portal apps landing page|
|lastModifiedDateTime|DateTimeOffset|Time when the BrandingProfile was last modified|
|lightBackgroundLogo|[mimeContent](../resources/mimecontent.md)|Logo image displayed in Company Portal apps which have a light background behind the logo|
|onlineSupportSiteName|String|Display name of the company/organization’s IT helpdesk site|
|onlineSupportSiteUrl|String|URL to the company/organization’s IT helpdesk site|
|privacyUrl|String|URL to the company/organization’s privacy policy|
|profileDescription|String|Description of the profile|
|profileName|String|Name of the profile|
|roleScopeTagIds|String collection|List of scope tags assigned to the branding profile|
|sendDeviceOwnershipChangePushNotification|Boolean|Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate|
|showAzureADEnterpriseApps|Boolean|Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal|
|showDisplayNameNextToLogo|Boolean|Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not|
|showLogo|Boolean|Boolean that represents whether the administrator-supplied logo images are shown or not|
|showOfficeWebApps|Boolean|Boolean that indicates if Office WebApps will be shown in Company Portal|
|themeColor|[rgbColor](../resources/rgbcolor.md)|Primary theme color used in the Company Portal applications and web portal|
|themeColorLogo|[mimeContent](../resources/mimecontent.md)|Logo image displayed in Company Portal apps which have a theme color background behind the logo|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) collection|The list of group assignments for the branding profile|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "String (identifier)",
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction"
    }
  ],
  "contactITEmailAddress": "String",
  "contactITName": "String",
  "contactITNotes": "String",
  "contactITPhoneNumber": "String",
  "createdDateTime": "String (timestamp)",
  "customCanSeePrivacyMessage": "String",
  "customCantSeePrivacyMessage": "String",
  "customPrivacyMessage": "String",
  "disableClientTelemetry": "Boolean",
  "displayName": "String",
  "enrollmentAvailability": "String",
  "isDefaultProfile": "Boolean",
  "isFactoryResetDisabled": "Boolean",
  "isRemoveDeviceDisabled": "Boolean",
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "onlineSupportSiteName": "String",
  "onlineSupportSiteUrl": "String",
  "privacyUrl": "String",
  "profileDescription": "String",
  "profileName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "sendDeviceOwnershipChangePushNotification": "Boolean",
  "showAzureADEnterpriseApps": "Boolean",
  "showDisplayNameNextToLogo": "Boolean",
  "showLogo": "Boolean",
  "showOfficeWebApps": "Boolean",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor"
  },
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent"
  }
}
```

