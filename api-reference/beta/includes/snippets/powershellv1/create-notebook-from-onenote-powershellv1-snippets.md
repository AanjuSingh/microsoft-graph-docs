---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Notes

$params = @{
	DisplayName = "My Private notebook"
}

# A UPN can also be used as -UserId.
New-MgUserOnenoteNotebook -UserId $userId -BodyParameter $params

```