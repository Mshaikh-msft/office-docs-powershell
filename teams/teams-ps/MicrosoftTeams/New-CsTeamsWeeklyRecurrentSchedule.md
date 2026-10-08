---
applicable: Microsoft Teams
author: officedocspr
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: bulenteg
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/new-csteamsweeklyrecurrentschedule
schema: 2.0.0
title: New-CsTeamsWeeklyRecurrentSchedule
---
# New-CsTeamsWeeklyRecurrentSchedule
## SYNOPSIS
Creates a weekly recurrent schedule definition.
## SYNTAX
```
New-CsTeamsWeeklyRecurrentSchedule [-MondayHours <object[]>] [-TuesdayHours <object[]>] [-WednesdayHours <object[]>] [-ThursdayHours <object[]>] [-FridayHours <object[]>] [-SaturdayHours <object[]>] [-SundayHours <object[]>] [-Complement] [<CommonParameters>]
```
## DESCRIPTION
Creates a weekly recurrence from weekday time ranges. Use `-Complement` to invert the specified hours.
## EXAMPLES
```powershell
$range = New-CsTeamsTimeRange -Start "09:00" -End "17:00"
$recurrence = New-CsTeamsWeeklyRecurrentSchedule -MondayHours @($range) -TuesdayHours @($range) -WednesdayHours @($range) -ThursdayHours @($range) -FridayHours @($range)
```
## PARAMETERS
### -MondayHours
Specifies Monday time ranges.
### -TuesdayHours
Specifies Tuesday time ranges.
### -WednesdayHours
Specifies Wednesday time ranges.
### -ThursdayHours
Specifies Thursday time ranges.
### -FridayHours
Specifies Friday time ranges.
### -SaturdayHours
Specifies Saturday time ranges.
### -SundayHours
Specifies Sunday time ranges.
### -Complement
Inverts the specified weekday time ranges.
### CommonParameters
This cmdlet supports the common parameters.
