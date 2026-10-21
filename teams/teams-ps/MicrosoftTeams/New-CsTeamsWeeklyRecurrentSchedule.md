---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: mshaikh
online version: https://learn.microsoft.com/powershell/module/microsoftteams/new-csteamsweeklyrecurrentschedule
schema: 2.0.0
title: New-CsTeamsWeeklyRecurrentSchedule
---
# New-CsTeamsWeeklyRecurrentSchedule
## SYNOPSIS
Creates a weekly recurrent schedule definition.
## SYNTAX
```
New-CsTeamsWeeklyRecurrentSchedule [-Monday <object[]>] [-Tuesday <object[]>] [-Wednesday <object[]>] [-Thursday <object[]>] [-Friday <object[]>] [-Saturday <object[]>] [-Sunday <object[]>] -Complement <bool> [<CommonParameters>]
```
## DESCRIPTION
Creates a weekly recurrence from weekday time ranges. Use `-Complement $false` to use the specified hours or `-Complement $true` to invert them.
## EXAMPLES
```powershell
$range = New-CsTeamsTimeRange -Start "09:00" -End "17:00"
$recurrence = New-CsTeamsWeeklyRecurrentSchedule -Monday @($range) -Complement $false
```
## PARAMETERS
### -Monday
Specifies Monday time ranges.
### -Tuesday
Specifies Tuesday time ranges.
### -Wednesday
Specifies Wednesday time ranges.
### -Thursday
Specifies Thursday time ranges.
### -Friday
Specifies Friday time ranges.
### -Saturday
Specifies Saturday time ranges.
### -Sunday
Specifies Sunday time ranges.
### -Complement
Specifies whether to invert the specified weekday time ranges.
### CommonParameters
This cmdlet supports the common parameters.
