---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ItemEmail
{
	DisplayName = "Business Email",
	Type = "work",
};
await graphClient.Users["user-id"].Profile.Emails["itemEmail-id"].PatchAsync(requestBody);


```