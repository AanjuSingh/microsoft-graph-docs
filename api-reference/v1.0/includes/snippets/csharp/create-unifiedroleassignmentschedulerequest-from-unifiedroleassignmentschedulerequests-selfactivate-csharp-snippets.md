---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnifiedRoleAssignmentScheduleRequest
{
	Action = "selfActivate",
	PrincipalId = "071cc716-8147-4397-a5ba-b2105951cc0b",
	RoleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4",
	DirectoryScopeId = "/",
	Justification = "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs",
	ScheduleInfo = new RequestSchedule
	{
		StartDateTime = DateTimeOffset.Parse("2022-04-14T00:00:00.000Z"),
		Expiration = new ExpirationPattern
		{
			Type = "AfterDuration",
			Duration = "PT5H",
		},
	},
	TicketInfo = new TicketInfo
	{
		TicketNumber = "CONTOSO:Normal-67890",
		TicketSystem = "MS Project",
	},
};
var result = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests.PostAsync(requestBody);


```