---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new User
{
	OnPremisesExtensionAttributes = new OnPremisesExtensionAttributes
	{
		ExtensionAttribute1 = "skypeId.adeleVance",
		ExtensionAttribute13 = null,
	},
};
var result = await graphClient.Users["user-id"].PatchAsync(requestBody);


```