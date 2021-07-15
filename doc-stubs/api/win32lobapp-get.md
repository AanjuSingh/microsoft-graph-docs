---
title: "Get win32LobApp"
description: "Read the properties and relationships of a win32LobApp object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get win32LobApp
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [win32LobApp](../resources/win32lobapp.md) object.

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
GET ** Entity URI for microsoft.graph.win32LobApp not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [win32LobApp](../resources/win32lobapp.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_win32lobapp"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.graph.win32LobApp not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.win32LobApp"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.win32LobApp",
    "id": "89e0a075-a075-89e0-75a0-e08975a0e089",
    "createdDateTime": "String (timestamp)",
    "dependentAppCount": "Integer",
    "description": "String",
    "developer": "String",
    "displayName": "String",
    "informationUrl": "String",
    "isAssigned": "Boolean",
    "isFeatured": "Boolean",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "notes": "String",
    "owner": "String",
    "privacyInformationUrl": "String",
    "publisher": "String",
    "publishingState": "String",
    "roleScopeTagIds": [
      "String"
    ],
    "supersededAppCount": "Integer",
    "supersedingAppCount": "Integer",
    "uploadState": "Integer",
    "committedContentVersion": "String",
    "fileName": "String",
    "size": "Integer",
    "applicableArchitectures": "String",
    "detectionRules": [
      {
        "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
      }
    ],
    "displayVersion": "String",
    "installCommandLine": "String",
    "installExperience": {
      "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
    },
    "minimumCpuSpeedInMHz": "Integer",
    "minimumFreeDiskSpaceInMB": "Integer",
    "minimumMemoryInMB": "Integer",
    "minimumNumberOfProcessors": "Integer",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
    },
    "minimumSupportedWindowsRelease": "String",
    "msiInformation": {
      "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
    },
    "requirementRules": [
      {
        "@odata.type": "microsoft.graph.win32LobAppFileSystemRequirement"
      }
    ],
    "returnCodes": [
      {
        "@odata.type": "microsoft.graph.win32LobAppReturnCode"
      }
    ],
    "rules": [
      {
        "@odata.type": "microsoft.graph.win32LobAppFileSystemRule"
      }
    ],
    "setupFilePath": "String",
    "uninstallCommandLine": "String"
  }
}
```

