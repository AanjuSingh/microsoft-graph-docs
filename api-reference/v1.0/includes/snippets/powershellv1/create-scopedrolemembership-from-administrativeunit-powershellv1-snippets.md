---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	RoleId = "roleId-value"
	RoleMemberInfo = @{
		Id = "id-value"
	}
}

New-MgDirectoryAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```