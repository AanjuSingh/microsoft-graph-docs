---
title: "alertRecord: setPortalNotificationAsSent"
description: "Set a single portal notification status to published. Will set isPortalNotificationSent property to true for current user."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: apiPageType
---

# alertRecord: setPortalNotificationAsSent
Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Set a single portal notification status to published. Will set isPortalNotificationSent property to true for current user.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|CloudPC.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|CloudPC.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/monitoring/alertRecords/{alertRecordId}/setPortalNotificationAsSent
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "alertrecordthis.setportalnotificationassent"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/monitoring/alertRecords/{alertRecordId}/setPortalNotificationAsSent
```


### Response
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
