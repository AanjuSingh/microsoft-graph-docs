---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new GroupSetting
{
	Values = new List<SettingValue>
	{
		new SettingValue
		{
			AdditionalData = new()
			{
				{"name", "AllowToAddGuests"},
				{"value", "false"},
			}
		},
	}
};
await graphClient.GroupSettings["groupSetting-id"].PatchAsync(requestBody);


```