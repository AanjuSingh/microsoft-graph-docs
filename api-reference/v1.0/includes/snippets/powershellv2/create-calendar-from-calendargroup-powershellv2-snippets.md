---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Calendar

$params = @{
	name = "Marketing calendar"
}

# A UPN can also be used as -UserId.
New-MgUserCalendarGroupCalendar -UserId $userId -CalendarGroupId $calendarGroupId -BodyParameter $params

```