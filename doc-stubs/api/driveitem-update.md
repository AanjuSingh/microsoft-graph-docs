---
title: "Update driveItem"
description: "Update the properties of a driveItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update driveItem
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [driveItem](../resources/driveitem.md) object.

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
PATCH /drive/root
PATCH /drives/{drivesId}/root
PATCH /shares/{sharesId}/root
PATCH /drive/items/{driveItemId}
PATCH /shares/{sharesId}/driveItem
PATCH /drive/bundles/{driveItemId}
PATCH /drive/special/{driveItemId}
PATCH /drive/following/{driveItemId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/intune-identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md). Optional.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md). Required.|
|description|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md). Optional.|
|eTag|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md). Optional.|
|lastModifiedBy|[identitySet](../resources/intune-identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md). Optional.|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md). Required.|
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md). Optional.|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md). Optional.|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md). Optional.|
|audio|[audio](../resources/audio.md)|**TODO: Add Description** Optional.|
|bundle|[bundle](../resources/bundle.md)|**TODO: Add Description** Optional.|
|content|Stream|**TODO: Add Description** Optional.|
|cTag|String|**TODO: Add Description** Optional.|
|deleted|[deleted](../resources/deleted.md)|**TODO: Add Description** Optional.|
|file|[file](../resources/file.md)|**TODO: Add Description** Optional.|
|fileSystemInfo|[fileSystemInfo](../resources/filesysteminfo.md)|**TODO: Add Description** Optional.|
|folder|[folder](../resources/folder.md)|**TODO: Add Description** Optional.|
|image|[image](../resources/image.md)|**TODO: Add Description** Optional.|
|location|[geoCoordinates](../resources/geocoordinates.md)|**TODO: Add Description** Optional.|
|malware|[malware](../resources/malware.md)|**TODO: Add Description** Optional.|
|media|[media](../resources/media.md)|**TODO: Add Description** Optional.|
|package|[package](../resources/package.md)|**TODO: Add Description** Optional.|
|pendingOperations|[pendingOperations](../resources/pendingoperations.md)|**TODO: Add Description** Optional.|
|photo|[photo](../resources/photo.md)|**TODO: Add Description** Optional.|
|publication|[publicationFacet](../resources/publicationfacet.md)|**TODO: Add Description** Optional.|
|remoteItem|[remoteItem](../resources/remoteitem.md)|**TODO: Add Description** Optional.|
|root|[root](../resources/root.md)|**TODO: Add Description** Optional.|
|searchResult|[searchResult](../resources/searchresult.md)|**TODO: Add Description** Optional.|
|shared|[shared](../resources/shared.md)|**TODO: Add Description** Optional.|
|sharepointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description** Optional.|
|size|Int64|**TODO: Add Description** Optional.|
|source|[driveItemSource](../resources/driveitemsource.md)|**TODO: Add Description** Optional.|
|specialFolder|[specialFolder](../resources/specialfolder.md)|**TODO: Add Description** Optional.|
|video|[video](../resources/video.md)|**TODO: Add Description** Optional.|
|webDavUrl|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [driveItem](../resources/driveitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_driveitem"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/drive/root
Content-Type: application/json
Content-length: 1953

{
  "@odata.type": "#microsoft.graph.driveItem",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": "String",
  "eTag": "String",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "webUrl": "String",
  "audio": {
    "@odata.type": "microsoft.graph.audio"
  },
  "bundle": {
    "@odata.type": "microsoft.graph.bundle"
  },
  "content": "Stream",
  "cTag": "String",
  "deleted": {
    "@odata.type": "microsoft.graph.deleted"
  },
  "file": {
    "@odata.type": "microsoft.graph.file"
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder"
  },
  "image": {
    "@odata.type": "microsoft.graph.image"
  },
  "location": {
    "@odata.type": "microsoft.graph.geoCoordinates"
  },
  "malware": {
    "@odata.type": "microsoft.graph.malware"
  },
  "media": {
    "@odata.type": "microsoft.graph.media"
  },
  "package": {
    "@odata.type": "microsoft.graph.package"
  },
  "pendingOperations": {
    "@odata.type": "microsoft.graph.pendingOperations"
  },
  "photo": {
    "@odata.type": "microsoft.graph.photo"
  },
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "remoteItem": {
    "@odata.type": "microsoft.graph.remoteItem"
  },
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "searchResult": {
    "@odata.type": "microsoft.graph.searchResult"
  },
  "shared": {
    "@odata.type": "microsoft.graph.shared"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "size": "Integer",
  "source": {
    "@odata.type": "microsoft.graph.driveItemSource"
  },
  "specialFolder": {
    "@odata.type": "microsoft.graph.specialFolder"
  },
  "video": {
    "@odata.type": "microsoft.graph.video"
  },
  "webDavUrl": "String"
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
  "@odata.type": "#microsoft.graph.driveItem",
  "id": "0f963543-3543-0f96-4335-960f4335960f",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "eTag": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "webUrl": "String",
  "audio": {
    "@odata.type": "microsoft.graph.audio"
  },
  "bundle": {
    "@odata.type": "microsoft.graph.bundle"
  },
  "content": "Stream",
  "cTag": "String",
  "deleted": {
    "@odata.type": "microsoft.graph.deleted"
  },
  "file": {
    "@odata.type": "microsoft.graph.file"
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder"
  },
  "image": {
    "@odata.type": "microsoft.graph.image"
  },
  "location": {
    "@odata.type": "microsoft.graph.geoCoordinates"
  },
  "malware": {
    "@odata.type": "microsoft.graph.malware"
  },
  "media": {
    "@odata.type": "microsoft.graph.media"
  },
  "package": {
    "@odata.type": "microsoft.graph.package"
  },
  "pendingOperations": {
    "@odata.type": "microsoft.graph.pendingOperations"
  },
  "photo": {
    "@odata.type": "microsoft.graph.photo"
  },
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "remoteItem": {
    "@odata.type": "microsoft.graph.remoteItem"
  },
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "searchResult": {
    "@odata.type": "microsoft.graph.searchResult"
  },
  "shared": {
    "@odata.type": "microsoft.graph.shared"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "size": "Integer",
  "source": {
    "@odata.type": "microsoft.graph.driveItemSource"
  },
  "specialFolder": {
    "@odata.type": "microsoft.graph.specialFolder"
  },
  "video": {
    "@odata.type": "microsoft.graph.video"
  },
  "webDavUrl": "String"
}
```

