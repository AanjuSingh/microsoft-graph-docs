---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityProvider
{
	@odata.type = "microsoft.graph.openIdConnectProvider",
	Name = "Login with the Contoso identity provider",
	Type = "OpenIDConnect",
	ClientId = "56433757-cadd-4135-8431-2c9e3fd68ae8",
	ClientSecret = "12345",
	AdditionalData = new()
	{
		{"domainHint", "mycustomoidc"},
		{"metadataUrl", "https://mycustomoidc.com/.well-known/openid-configuration"},
		{"responseMode", "form_post"},
		{"responseType", "code"},
		{"scope", "openid"},
	}
};
var result = await graphClient.IdentityProviders.PostAsync(requestBody);


```