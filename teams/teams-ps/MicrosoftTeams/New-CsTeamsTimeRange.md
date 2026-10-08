---
applicable: Microsoft Teams
author: officedocspr
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: bulenteg
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/new-csteamstimerange
schema: 2.0.0
title: New-CsTeamsTimeRange
---
# New-CsTeamsTimeRange
## SYNOPSIS
Creates a time range for a Teams schedule.
## SYNTAX
```
New-CsTeamsTimeRange -Start <datetime> -End <datetime> [<CommonParameters>]
```
## DESCRIPTION
Creates a time range with a start and end time.
## EXAMPLES
```powershell
$range = New-CsTeamsTimeRange -Start "09:00" -End "17:00"
```
## PARAMETERS
### -Start
Specifies the starting time.
### -End
Specifies the ending time.
### CommonParameters
This cmdlet supports the common parameters.
