---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	name = "Connector Group Demo"
}

New-MgBetaOnPremisePublishingProfileConnectorGroup -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -BodyParameter $params

```