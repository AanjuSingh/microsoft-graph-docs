---
title: "Create sharedEmailDomainInvitation"
description: "Create a new sharedEmailDomainInvitation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create sharedEmailDomainInvitation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new sharedEmailDomainInvitation object.

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
POST /domains/{domainsId}/sharedEmailDomainInvitations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [sharedEmailDomainInvitation](../resources/sharedemaildomaininvitation.md) object.

The following table shows the properties that are required when you create the [sharedEmailDomainInvitation](../resources/sharedemaildomaininvitation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|expiryTime|DateTimeOffset|**TODO: Add Description**|
|invitationDomain|String|**TODO: Add Description**|
|invitationStatus|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [sharedEmailDomainInvitation](../resources/sharedemaildomaininvitation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_sharedemaildomaininvitation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/domains/{domainsId}/sharedEmailDomainInvitations
Content-Type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.sharedEmailDomainInvitation",
  "expiryTime": "String (timestamp)",
  "invitationDomain": "String",
  "invitationStatus": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedEmailDomainInvitation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.sharedEmailDomainInvitation",
  "id": "71e9d534-d534-71e9-34d5-e97134d5e971",
  "expiryTime": "String (timestamp)",
  "invitationDomain": "String",
  "invitationStatus": "String"
}
```

