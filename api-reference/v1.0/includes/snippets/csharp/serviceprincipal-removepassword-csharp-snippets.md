---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new KeyIdRequestBody
{
	KeyId = "f0b0b335-1d71-4883-8f98-567911bfdca6",
};
await graphClient.ServicePrincipals["servicePrincipal-id"].RemovePassword.PostAsync(requestBody);


```