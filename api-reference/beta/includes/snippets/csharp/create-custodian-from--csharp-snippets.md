---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Custodian
{
	Email = "AdeleV@contoso.com",
	ApplyHoldToSources = "true",
};
var result = await graphClient.Compliance.Ediscovery.Cases["case-id"].Custodians.PostAsync(requestBody);


```