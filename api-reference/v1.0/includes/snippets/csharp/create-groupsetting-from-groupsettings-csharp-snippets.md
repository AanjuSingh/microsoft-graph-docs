---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new GroupSetting
{
	TemplateId = "62375ab9-6b52-47ed-826b-58e47e0e304b",
	Values = new List<SettingValue>
	{
		new SettingValue
		{
			AdditionalData = new()
			{
				{"name", "GuestUsageGuidelinesUrl"},
				{"value", "https://privacy.contoso.com/privacystatement"},
			}
		},
		new SettingValue
		{
			AdditionalData = new()
			{
				{"name", "EnableMSStandardBlockedWords"},
				{"value", "true"},
			}
		},
		new SettingValue
		{
			AdditionalData = new()
			{
				{"name", "EnableMIPLabels"},
				{"value", "true"},
			}
		},
		new SettingValue
		{
			AdditionalData = new()
			{
				{"name", "PrefixSuffixNamingRequirement"},
				{"value", "[Contoso-][GroupName]"},
			}
		},
	}
};
var result = await graphClient.GroupSettings.PostAsync(requestBody);


```