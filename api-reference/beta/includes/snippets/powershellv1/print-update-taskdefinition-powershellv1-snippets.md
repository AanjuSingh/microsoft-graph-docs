---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
	DisplayName = "Test TaskDefinitionName"
	CreatedBy = @{
		DisplayName = "Requesting App Display Name"
	}
}

Update-MgPrintTaskDefinition -PrintTaskDefinitionId $printTaskDefinitionId -BodyParameter $params

```