---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new GetScheduleRequestBody
{
	Schedules = new List<String>
	{
		"adelev@contoso.onmicrosoft.com",
		"meganb@contoso.onmicrosoft.com",
	}
	StartTime = new DateTimeTimeZone
	{
		DateTime = "2019-03-15T09:00:00",
		TimeZone = "Pacific Standard Time",
	},
	EndTime = new DateTimeTimeZone
	{
		DateTime = "2019-03-15T18:00:00",
		TimeZone = "Pacific Standard Time",
	},
	AvailabilityViewInterval = 60,
};
var result = await graphClient.Me.Calendar.GetSchedule.PostAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "outlook.timezone="Pacific Standard Time"");
});


```