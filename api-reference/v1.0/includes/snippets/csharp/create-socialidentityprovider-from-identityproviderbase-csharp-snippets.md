---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityProviderBase
{
	@odata.type = "microsoft.graph.socialIdentityProvider",
	DisplayName = "Login with Amazon",
	AdditionalData = new()
	{
		{"identityProviderType", "Amazon"},
		{"clientId", "56433757-cadd-4135-8431-2c9e3fd68ae8"},
		{"clientSecret", "000000000000"},
	}
};
var result = await graphClient.Identity.IdentityProviders.PostAsync(requestBody);


```