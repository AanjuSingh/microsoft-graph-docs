---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PhoneAuthenticationMethod-idRequestBody
{
	AdditionalData = new()
	{
		{"phoneNumber", "+1 2065555554"},
		{"phoneType", "mobile"},
	}
};
await graphClient.Me.Authentication.PhoneMethods["phoneAuthenticationMethod-id"].PutAsync(requestBody);


```