---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EmailAuthenticationMethod-idRequestBody
{
	AdditionalData = new()
	{
		{"emailAddress", "kim@contoso.com"},
	}
};
await graphClient.Users["user-id"].Authentication.EmailMethods["emailAuthenticationMethod-id"].PutAsync(requestBody);


```