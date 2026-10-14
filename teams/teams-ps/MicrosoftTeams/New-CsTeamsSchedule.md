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
New-CsTeamsSchedule -WeeklyRecurrenceHours <object> [<CommonParameters>]
```
## DESCRIPTION
Creates a schedule from a weekly recurrence.
## EXAMPLES
```powershell
$range = New-CsTeamsTimeRange -Start "09:00" -End "17:00"
$recurrence = New-CsTeamsWeeklyRecurrentSchedule -Monday @($range) -Complement $false
$schedule = New-CsTeamsSchedule -WeeklyRecurrenceHours $recurrence
```
## PARAMETERS
### -WeeklyRecurrenceHours
Specifies the weekly recurrence object.
### CommonParameters
This cmdlet supports the common parameters.
