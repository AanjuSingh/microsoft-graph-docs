---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Security

$params = @{
	AssignedTo = ""
	Comment = "control is reviewed"
	State = "Reviewed"
	VendorInformation = @{
		Provider = "SecureScore"
		ProviderVersion = $null
		SubProvider = $null
		Vendor = "Microsoft"
	}
}

Update-MgSecuritySecureScoreControlProfile -SecureScoreControlProfileId $secureScoreControlProfileId -BodyParameter $params

```