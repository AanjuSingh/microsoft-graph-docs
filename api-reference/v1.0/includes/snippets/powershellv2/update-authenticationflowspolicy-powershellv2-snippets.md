---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	selfServiceSignUp = @{
		isEnabled = $true
	}
}

Update-MgPolicyAuthenticationFlowPolicy -BodyParameter $params

```