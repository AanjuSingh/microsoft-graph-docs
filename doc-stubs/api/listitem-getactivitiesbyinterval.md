---
title: "listItem: getActivitiesByInterval"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# listItem: getActivitiesByInterval
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
GET /shares/{sharesId}/listItem/getActivitiesByInterval
GET /workbooks/{workbooksId}/listItem/getActivitiesByInterval
```

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|startDateTime|String|**TODO: Add Description**|
|endDateTime|String|**TODO: Add Description**|
|interval|String|**TODO: Add Description**|


## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [itemActivityStat](../resources/itemactivitystat.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "listitem_getactivitiesbyinterval"
}
-->
``` http
GET https://graph.microsoft.com/beta/shares/{sharesId}/listItem/getActivitiesByInterval(startDateTime='parameterValue',endDateTime='parameterValue',interval='parameterValue')
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.itemActivityStat)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.itemActivityStat",
      "id": "String (identifier)",
      "access": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "create": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "delete": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "edit": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "endDateTime": "String (timestamp)",
      "incompleteData": {
        "@odata.type": "microsoft.graph.incompleteData"
      },
      "isTrending": "Boolean",
      "move": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "startDateTime": "String (timestamp)"
    }
  ]
}
```

