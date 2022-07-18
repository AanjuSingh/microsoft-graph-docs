---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityProviderBase-idRequestBody
{
	AdditionalData = new()
	{
		{"@odata.id", "https://graph.microsoft.com/beta/identity/identityProviders/{id}"},
		{"@odata.type", "#microsoft.graph.identityProvider"},
	}
};
await graphClient.Identity.B2cUserFlows["b2cIdentityUserFlow-id"].UserFlowIdentityProviders["identityProviderBase-id"].PatchAsync(requestBody);


```