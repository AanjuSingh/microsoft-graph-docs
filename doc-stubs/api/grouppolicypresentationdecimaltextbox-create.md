---
title: "Create groupPolicyPresentationDecimalTextBox"
description: "Create a new groupPolicyPresentationDecimalTextBox object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create groupPolicyPresentationDecimalTextBox
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [groupPolicyPresentationDecimalTextBox](../resources/grouppolicypresentationdecimaltextbox.md) object.

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
POST ** Collection URI for microsoft.graph.groupPolicyPresentationDecimalTextBox not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupPolicyPresentationDecimalTextBox](../resources/grouppolicypresentationdecimaltextbox.md) object.

The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/grouppolicypresentationdecimaltextbox.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|defaultValue|Int64|An unsigned integer that specifies the initial value for the decimal text box. The default value is 1.|
|maxValue|Int64|An unsigned integer that specifies the maximum allowed value. The default value is 9999.|
|minValue|Int64|An unsigned integer that specifies the minimum allowed value. The default value is 0.|
|required|Boolean|Requirement to enter a value in the parameter box. The default value is false.|
|spin|Boolean|If true, create a spin control; otherwise, create a text box for numeric entry. The default value is true.|
|spinStep|Int64|An unsigned integer that specifies the increment of change for the spin control. The default value is 1.|



## Response

If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDecimalTextBox](../resources/grouppolicypresentationdecimaltextbox.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_grouppolicypresentationdecimaltextbox_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.groupPolicyPresentationDecimalTextBox not found
Content-Type: application/json
Content-length: 257

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "String",
  "defaultValue": "Integer",
  "maxValue": "Integer",
  "minValue": "Integer",
  "required": "Boolean",
  "spin": "Boolean",
  "spinStep": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupPolicyPresentationDecimalTextBox"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "id": "6709c2d9-c2d9-6709-d9c2-0967d9c20967",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "Integer",
  "maxValue": "Integer",
  "minValue": "Integer",
  "required": "Boolean",
  "spin": "Boolean",
  "spinStep": "Integer"
}
```

