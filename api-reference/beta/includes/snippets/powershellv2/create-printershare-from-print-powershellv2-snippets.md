---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Devices.CloudPrint

$params = @{
	name = "name-value"
	"printer@odata.bind" = "https://graph.microsoft.com/beta/print/printers/{id}"
}

New-MgBetaPrintShare -BodyParameter $params

```