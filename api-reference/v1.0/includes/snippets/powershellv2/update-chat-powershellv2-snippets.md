---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Teams

$params = @{
	topic = "Group chat title update"
}

Update-MgChat -ChatId $chatId -BodyParameter $params

```