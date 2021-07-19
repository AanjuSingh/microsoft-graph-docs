---
title: "Get servicePrincipal"
description: "Read the properties and relationships of a servicePrincipal object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get servicePrincipal
Namespace: microsoft.graph



Read the properties and relationships of a [servicePrincipal](../resources/serviceprincipal.md) object.

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
GET /servicePrincipals/{servicePrincipalsId}
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

If successful, this method returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{servicePrincipalsId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.servicePrincipal",
    "id": "3cdf958e-958e-3cdf-8e95-df3c8e95df3c",
    "deletedDateTime": "String (timestamp)",
    "accountEnabled": "Boolean",
    "addIns": [
      {
        "@odata.type": "microsoft.graph.addIn"
      }
    ],
    "alternativeNames": [
      "String"
    ],
    "appDescription": "String",
    "appDisplayName": "String",
    "appId": "String",
    "applicationTemplateId": "String",
    "appOwnerOrganizationId": "Guid",
    "appRoleAssignmentRequired": "Boolean",
    "appRoles": [
      {
        "@odata.type": "microsoft.graph.appRole"
      }
    ],
    "description": "String",
    "disabledByMicrosoftStatus": "String",
    "displayName": "String",
    "hasPermissionClassifications": "Boolean",
    "homepage": "String",
    "info": {
      "@odata.type": "microsoft.graph.informationalUrl"
    },
    "keyCredentials": [
      {
        "@odata.type": "microsoft.graph.keyCredential"
      }
    ],
    "loginUrl": "String",
    "logoutUrl": "String",
    "notes": "String",
    "notificationEmailAddresses": [
      "String"
    ],
    "oauth2PermissionScopes": [
      {
        "@odata.type": "microsoft.graph.permissionScope"
      }
    ],
    "passwordCredentials": [
      {
        "@odata.type": "microsoft.graph.passwordCredential"
      }
    ],
    "preferredSingleSignOnMode": "String",
    "preferredTokenSigningKeyThumbprint": "String",
    "replyUrls": [
      "String"
    ],
    "samlSingleSignOnSettings": {
      "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
    },
    "servicePrincipalNames": [
      "String"
    ],
    "servicePrincipalType": "String",
    "signInAudience": "String",
    "tags": [
      "String"
    ],
    "tokenEncryptionKeyId": "Guid"
  }
}
```

