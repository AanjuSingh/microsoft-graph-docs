---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ReferenceCreate
{
	@odata.id = "https://graph.microsoft.com/beta/education/users/14011",
};
await graphClient.Education.Classes["educationClass-id"].Teachers.$ref.PostAsync(requestBody);


```