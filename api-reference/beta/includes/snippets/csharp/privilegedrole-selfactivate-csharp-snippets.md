---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SelfActivateRequestBody
{
	Reason = "reason-value",
	Duration = "duration-value",
	TicketNumber = "ticketNumber-value",
	TicketSystem = "ticketSystem-value",
};
var result = await graphClient.PrivilegedRoles["privilegedRole-id"].SelfActivate.PostAsync(requestBody);


```