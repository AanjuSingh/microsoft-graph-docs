---
title: "Create groupPolicyPresentationMultiTextBox"
description: "Create a new groupPolicyPresentationMultiTextBox object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create groupPolicyPresentationMultiTextBox
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md) object.

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
POST ** Collection URI for microsoft.graph.groupPolicyPresentationMultiTextBox not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md) object.

The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|maxLength|Int64|An unsigned integer that specifies the maximum number of text characters. Default value is 1023.|
|maxStrings|Int64|An unsigned integer that specifies the maximum number of strings. Default value is 0.|
|required|Boolean|Requirement to enter a value in the text box. Default value is false.|



## Response

If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_grouppolicypresentationmultitextbox_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.groupPolicyPresentationMultiTextBox not found
Content-Type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "String",
  "maxLength": "Integer",
  "maxStrings": "Integer",
  "required": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupPolicyPresentationMultiTextBox"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "id": "66baebc2-ebc2-66ba-c2eb-ba66c2ebba66",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxLength": "Integer",
  "maxStrings": "Integer",
  "required": "Boolean"
}
```

