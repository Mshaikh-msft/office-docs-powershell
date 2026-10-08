---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/new-csteamsschedule
schema: 2.0.0
title: New-CsTeamsSchedule
---
# New-CsTeamsSchedule
## SYNOPSIS
Creates a Teams schedule.
## SYNTAX
```
New-CsTeamsSchedule -Name <string> -WeeklyRecurrence <object> [<CommonParameters>]
```
## DESCRIPTION
Creates a schedule from a weekly recurrence.
## EXAMPLES
```powershell
$recurrence = New-CsTeamsWeeklyRecurrentSchedule -MondayHours @($range)
New-CsTeamsSchedule -Name "BusinessHours" -WeeklyRecurrence $recurrence
```
## PARAMETERS
### -Name
Specifies the unique schedule name.
### -WeeklyRecurrence
Specifies the weekly recurrence object.
### CommonParameters
This cmdlet supports the common parameters.
