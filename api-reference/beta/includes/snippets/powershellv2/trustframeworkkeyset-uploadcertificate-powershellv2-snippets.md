---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	key = "key-value"
}

Invoke-MgBetaUploadTrustFrameworkKeySetCertificate -TrustFrameworkKeySetId $trustFrameworkKeySetId -BodyParameter $params

```