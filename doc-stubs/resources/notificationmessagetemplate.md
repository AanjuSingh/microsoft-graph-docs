---
title: "notificationMessageTemplate resource type"
description: "Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator. Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section. Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# notificationMessageTemplate resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator. Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section. Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List notificationMessageTemplates](../api/notificationmessagetemplate-list.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md) collection|Get a list of the [notificationMessageTemplate](../resources/notificationmessagetemplate.md) objects and their properties.|
|[Create notificationMessageTemplate](../api/notificationmessagetemplate-create.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md)|Create a new [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.|
|[Get notificationMessageTemplate](../api/notificationmessagetemplate-get.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md)|Read the properties and relationships of a [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.|
|[Update notificationMessageTemplate](../api/notificationmessagetemplate-update.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md)|Update the properties of a [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.|
|[Delete notificationMessageTemplate](../api/notificationmessagetemplate-delete.md)|None|Deletes a [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.|
|[sendTestMessage](../api/notificationmessagetemplate-sendtestmessage.md)|None|Sends test message using the specified notificationMessageTemplate in the default locale|
|[List localizedNotificationMessages](../api/notificationmessagetemplate-list-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md) collection|Get the localizedNotificationMessage resources from the localizedNotificationMessages navigation property.|
|[Create localizedNotificationMessage](../api/notificationmessagetemplate-post-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Create a new localizedNotificationMessage object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|brandingOptions|notificationTemplateBrandingOptions|The Message Template Branding Options. Branding is defined in the Intune Admin Console. Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.|
|defaultLocale|String|The default locale to fallback onto when the requested locale is not available.|
|displayName|String|Display name for the Notification Message Template.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|localizedNotificationMessages|[localizedNotificationMessage](../resources/localizednotificationmessage.md) collection|The list of localized messages for this Notification Message Template.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "brandingOptions": "String",
  "defaultLocale": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```

