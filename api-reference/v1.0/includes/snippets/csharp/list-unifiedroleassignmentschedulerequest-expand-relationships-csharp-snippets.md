---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Select = new [] { "principalId" , "action" , "roleDefinitionId" };
	requestConfiguration.QueryParameters.Expand = new [] { "roleDefinition" , "activatedUsing" , "principal" , "targetSchedule" };
});


```