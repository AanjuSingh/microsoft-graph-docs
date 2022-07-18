---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Extension
{
	@odata.type = "microsoft.graph.openTypeExtension",
	AdditionalData = new()
	{
		{"extensionName", "Com.Contoso.Referral"},
		{"companyName", "Wingtip Toys"},
		{"dealValue", },
		{"expirationDate", "2015-12-03T10:00:00.000Z"},
	}
};
var result = await graphClient.Me.Messages["message-id"].Extensions.PostAsync(requestBody);


```