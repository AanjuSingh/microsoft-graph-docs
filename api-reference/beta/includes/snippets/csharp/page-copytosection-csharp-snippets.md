---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CopyToSectionRequestBody
{
	Id = "id-value",
	GroupId = "groupId-value",
};
var result = await graphClient.Me.Onenote.Pages["onenotePage-id"].CopyToSection.PostAsync(requestBody);


```