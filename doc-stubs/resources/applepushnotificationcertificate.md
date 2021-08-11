---
title: "applePushNotificationCertificate resource type"
description: "Apple push notification certificate."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# applePushNotificationCertificate resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Apple push notification certificate.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List applePushNotificationCertificates](../api/applepushnotificationcertificate-list.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) collection|Get a list of the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) objects and their properties.|
|[Create applePushNotificationCertificate](../api/applepushnotificationcertificate-create.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)|Create a new [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[Get applePushNotificationCertificate](../api/applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)|Read the properties and relationships of an [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[Update applePushNotificationCertificate](../api/applepushnotificationcertificate-update.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)|Update the properties of an [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[Delete applePushNotificationCertificate](../api/applepushnotificationcertificate-delete.md)|None|Deletes an [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[downloadApplePushNotificationCertificateSigningRequest](../api/applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|String|Download Apple push notification certificate signing request|
|[generateApplePushNotificationCertificateSigningRequest](../api/applepushnotificationcertificate-generateapplepushnotificationcertificatesigningrequest.md)|String|Download Apple push notification certificate signing request|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleIdentifier|String|Apple Id of the account used to create the MDM push certificate.|
|certificate|String|**TODO: Add Description**|
|certificateSerialNumber|String|Certificate serial number. This property is read-only.|
|certificateUploadFailureReason|String|The reason the certificate upload failed.|
|certificateUploadStatus|String|The certificate upload status.|
|expirationDateTime|DateTimeOffset|The expiration date and time for Apple push notification certificate.|
|id|String|Unique Identifier for the certificate|
|lastModifiedDateTime|DateTimeOffset|Last modified date and time for Apple push notification certificate.|
|topicIdentifier|String|Topic Id.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificateUploadStatus": "String",
  "certificateUploadFailureReason": "String",
  "certificateSerialNumber": "String",
  "certificate": "String"
}
```

