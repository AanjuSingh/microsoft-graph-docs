---
title: "Update teamsAppDefinition"
description: "Update the properties of a teamsAppDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update teamsAppDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [teamsAppDefinition](../resources/teamsappdefinition.md) object.

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
PATCH /chats/{chatsId}/installedApps/{teamsAppInstallationId}/teamsAppDefinition
PATCH /chats/{chatsId}/installedApps/{teamsAppInstallationId}/teamsApp/appDefinitions/{teamsAppDefinitionId}
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
|allowedInstallationScopes|teamsAppInstallationScopes|**TODO: Add Description**. The possible values are: `team`, `groupChat`, `personal`, `unknownFutureValue`. Optional.|
|azureADAppId|String|**TODO: Add Description** Optional.|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Optional.|
|description|String|**TODO: Add Description** Optional.|
|displayName|String|**TODO: Add Description** Optional.|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|publishingState|teamsAppPublishingState|**TODO: Add Description**. The possible values are: `submitted`, `rejected`, `published`, `unknownFutureValue`. Optional.|
|requiredResourceSpecificApplicationPermissions|String collection|**TODO: Add Description** Optional.|
|serializedInternalDefinition|String|**TODO: Add Description** Optional.|
|shortdescription|String|**TODO: Add Description** Optional.|
|teamsAppId|String|**TODO: Add Description** Optional.|
|version|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [teamsAppDefinition](../resources/teamsappdefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_teamsappdefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/chats/{chatsId}/installedApps/{teamsAppInstallationId}/teamsAppDefinition
Content-Type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.teamsAppDefinition",
  "allowedInstallationScopes": "String",
  "azureADAppId": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": "String",
  "displayName": "String",
  "publishingState": "String",
  "requiredResourceSpecificApplicationPermissions": [
    "String"
  ],
  "serializedInternalDefinition": "String",
  "shortdescription": "String",
  "teamsAppId": "String",
  "version": "String"
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
  "@odata.type": "#microsoft.graph.teamsAppDefinition",
  "id": "ff38e9c5-e9c5-ff38-c5e9-38ffc5e938ff",
  "allowedInstallationScopes": "String",
  "azureADAppId": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "publishingState": "String",
  "requiredResourceSpecificApplicationPermissions": [
    "String"
  ],
  "serializedInternalDefinition": "String",
  "shortdescription": "String",
  "teamsAppId": "String",
  "version": "String"
}
```

