---
title: "servicePrincipal: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# servicePrincipal: delta
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

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
GET /servicePrincipals/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.servicePrincipal)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.servicePrincipal",
      "id": "String (identifier)",
      "deletedDateTime": "String (timestamp)",
      "passwordSingleSignOnSettings": {
        "@odata.type": "microsoft.graph.passwordSingleSignOnSettings"
      },
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
      "errorUrl": "String",
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
      "passwordCredentials": [
        {
          "@odata.type": "microsoft.graph.passwordCredential"
        }
      ],
      "preferredSingleSignOnMode": "String",
      "preferredTokenSigningKeyEndDateTime": "String (timestamp)",
      "preferredTokenSigningKeyThumbprint": "String",
      "publishedPermissionScopes": [
        {
          "@odata.type": "microsoft.graph.permissionScope"
        }
      ],
      "publisherName": "String",
      "replyUrls": [
        "String"
      ],
      "samlMetadataUrl": "String",
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
  ]
}
```

