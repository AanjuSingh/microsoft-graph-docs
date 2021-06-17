---
title: "Create externalConnection"
description: "Create a new externalConnection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create externalConnection
Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new externalConnection object.

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
POST /external/connections
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [externalConnection](../resources/externalconnectors-externalconnection.md) object.

The following table shows the properties that are required when you create the [externalConnection](../resources/externalconnectors-externalconnection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/externalconnectors-entity.md)|
|activitySettings|[microsoft.graph.externalConnectors.activitySettings](../resources/externalconnectors-activitysettings.md)|**TODO: Add Description**|
|complianceSettings|[microsoft.graph.externalConnectors.complianceSettings](../resources/externalconnectors-compliancesettings.md)|**TODO: Add Description**|
|configuration|[microsoft.graph.externalConnectors.configuration](../resources/externalconnectors-configuration.md)|**TODO: Add Description**|
|connectorId|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|searchSettings|[microsoft.graph.externalConnectors.searchSettings](../resources/externalconnectors-searchsettings.md)|**TODO: Add Description**|
|state|connectionState|**TODO: Add Description**. Possible values are: `draft`, `ready`, `obsolete`, `limitExceeded`, `unknownFutureValue`.|



## Response

If successful, this method returns a `201 Created` response code and an [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_externalconnection_from_connections"
}
-->
``` http
POST https://graph.microsoft.com/beta/external/connections
Content-Type: application/json
Content-length: 592

{
  "@odata.type": "#microsoft.graph.externalConnectors.externalConnection",
  "activitySettings": {
    "@odata.type": "microsoft.graph.externalConnectors.activitySettings"
  },
  "complianceSettings": {
    "@odata.type": "microsoft.graph.externalConnectors.complianceSettings"
  },
  "configuration": {
    "@odata.type": "microsoft.graph.externalConnectors.configuration"
  },
  "connectorId": "String",
  "description": "String",
  "name": "String",
  "searchSettings": {
    "@odata.type": "microsoft.graph.externalConnectors.searchSettings"
  },
  "state": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalConnectors.externalConnection",
  "id": "a5ecf050-f050-a5ec-50f0-eca550f0eca5",
  "activitySettings": {
    "@odata.type": "microsoft.graph.externalConnectors.activitySettings"
  },
  "complianceSettings": {
    "@odata.type": "microsoft.graph.externalConnectors.complianceSettings"
  },
  "configuration": {
    "@odata.type": "microsoft.graph.externalConnectors.configuration"
  },
  "connectorId": "String",
  "description": "String",
  "name": "String",
  "searchSettings": {
    "@odata.type": "microsoft.graph.externalConnectors.searchSettings"
  },
  "state": "String"
}
```

