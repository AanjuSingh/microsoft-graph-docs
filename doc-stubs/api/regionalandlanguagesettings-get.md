---
title: "Get regionalAndLanguageSettings"
description: "Read the properties and relationships of a regionalAndLanguageSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get regionalAndLanguageSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object.

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
GET /me/settings/regionalAndLanguageSettings
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

If successful, this method returns a `200 OK` response code and a [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_regionalandlanguagesettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/settings/regionalAndLanguageSettings
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.regionalAndLanguageSettings",
    "id": "846dd483-d483-846d-83d4-6d8483d46d84",
    "authoringLanguages": [
      {
        "@odata.type": "microsoft.graph.localeInfo"
      }
    ],
    "defaultDisplayLanguage": {
      "@odata.type": "microsoft.graph.localeInfo"
    },
    "defaultRegionalFormat": {
      "@odata.type": "microsoft.graph.localeInfo"
    },
    "defaultSpeechInputLanguage": {
      "@odata.type": "microsoft.graph.localeInfo"
    },
    "defaultTranslationLanguage": {
      "@odata.type": "microsoft.graph.localeInfo"
    },
    "regionalFormatOverrides": {
      "@odata.type": "microsoft.graph.regionalFormatOverrides"
    },
    "translationPreferences": {
      "@odata.type": "microsoft.graph.translationPreferences"
    }
  }
}
```

