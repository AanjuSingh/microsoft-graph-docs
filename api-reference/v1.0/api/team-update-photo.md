# Promoting change update the photo (picture) for a team from /beta to /v1.0
---
title: "Update team photo"
description: "Update the photo (picture) for a team."
author: "sumitgupta"
ms.localizationpriority: high
ms.prod: "microsoft-teams"
doc_type: apiPageType

---

# Update team photo

Namespace: microsoft.graph

Update the photo (picture) for a team.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | TeamSettingsReadWriteAll, GroupReadWriteAll**, DirectoryReadWriteAll** |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | TeamSettingsEditGroup*, TeamSettingsReadWriteGroup*, TeamSettingsReadWriteAll, GroupReadWriteAll**, DirectoryReadWriteAll** |

 **Notes**: 
> Permissions marked with ** are supported only for backward compatibility. We recommend that you update your solutions to use an alternative permission listed in the previous table and avoid using these permissions going forward. Permissions marked with * use [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).
>  This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.

## HTTP request

### Update the photo

This endpoint will update the binary data for the photo.

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /teams/{id}/photo/$value
```

## Request headers

| Header        | Value           |
|:--------------|:--------------  |
| Authorization | Bearer {token}. Required.  |

## Request body

Binary data of the image.
Content-type : image/jpeg

## Response

### Response for updating the photo

If successful, this method returns a `200 OK` response code.

## Examples

### Update the team photo

Here is an example of the request to update the team photo.

#### Request

<!-- {
  "blockType": "ignored",
  "name": "update_team_photo"
}-->
```http
PUT https://graph.microsoft.com/v1.0/teams/172b0cce-e65d-44ce-9a49-91d9f2e8491e/photo/$value
Content-type: image/jpeg

Binary data for the image
```

#### Response
```
HTTP/1.1 200 OK
```