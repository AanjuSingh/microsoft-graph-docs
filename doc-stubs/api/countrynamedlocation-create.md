---
title: "Create countryNamedLocation"
description: "Create a new countryNamedLocation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create countryNamedLocation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [countryNamedLocation](../resources/countrynamedlocation.md) object.

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
POST ** Collection URI for microsoft.graph.countryNamedLocation not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [countryNamedLocation](../resources/countrynamedlocation.md) object.

The following table shows the properties that are required when you create the [countryNamedLocation](../resources/countrynamedlocation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|displayName|String|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|countriesAndRegions|String collection|**TODO: Add Description**|
|countryLookupMethod|countryLookupMethodType|**TODO: Add Description**. Possible values are: `clientIpAddress`, `authenticatorAppGps`, `unknownFutureValue`.|
|includeUnknownCountriesAndRegions|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_countrynamedlocation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.countryNamedLocation not found
Content-Type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.countryNamedLocation",
  "displayName": "String",
  "countriesAndRegions": [
    "String"
  ],
  "countryLookupMethod": "String",
  "includeUnknownCountriesAndRegions": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryNamedLocation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.countryNamedLocation",
  "id": "6ab8ba3c-ba3c-6ab8-3cba-b86a3cbab86a",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "modifiedDateTime": "String (timestamp)",
  "countriesAndRegions": [
    "String"
  ],
  "countryLookupMethod": "String",
  "includeUnknownCountriesAndRegions": "Boolean"
}
```

