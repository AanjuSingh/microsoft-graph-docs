---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DisplayNameRequestBody
{
	DisplayName = "testProperties",
};
var result = await graphClient.ApplicationTemplates["applicationTemplate-id"].Instantiate.PostAsync(requestBody);


```