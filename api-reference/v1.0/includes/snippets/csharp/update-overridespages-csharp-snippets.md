---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new $valueRequestBody
{
	AdditionalData = new()
	{
		{"LocalizedStrings", new List<Object>
		{
		}
	}
};
await graphClient.Identity.B2xUserFlows["b2xIdentityUserFlow-id"].Languages["userFlowLanguageConfiguration-id"].OverridesPages["userFlowLanguagePage-id"].$value.PutAsync(requestBody);


```