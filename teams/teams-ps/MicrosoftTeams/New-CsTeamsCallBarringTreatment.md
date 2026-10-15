---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/new-csteamscallbarringtreatment
schema: 2.0.0
title: New-CsTeamsCallBarringTreatment
---
# New-CsTeamsCallBarringTreatment
## SYNOPSIS
Creates a Teams call barring treatment.
## SYNTAX
```
New-CsTeamsCallBarringTreatment -Identity <string> [-AllowedDestinations <string>] [-AllowedDestinationsPattern <string>] [-CallSource <string>] [-Schedule <object>] [-TimeZoneId <string>] [<CommonParameters>]
New-CsTeamsCallBarringTreatment -Parent <string> -Name <string> [-AllowedDestinations <string>] [-AllowedDestinationsPattern <string>] [-CallSource <string>] [-Schedule <object>] [-TimeZoneId <string>] [<CommonParameters>]
```
## DESCRIPTION
Creates a treatment under a dial-out policy. `CallSource` accepts `DialOut`, `ConferenceDialOut`, or `CallForwardSimRing`; `AllowedDestinations` accepts `None`, `DomesticOnly`, `ZoneA`, or `InternationalAndDomestic`. `ConferenceDialOut` requires `-Schedule $null`.
## EXAMPLES
### Example 1
```powershell
New-CsTeamsCallBarringTreatment -Parent "LobbyPhonePolicy" -Name "AfterHours" -AllowedDestinations "None" -CallSource "ConferenceDialOut" -Schedule $null
```
Creates a conference dial-out treatment.
## PARAMETERS
### -Identity
Specifies the combined policy and treatment identity.
### -Parent
Specifies the parent policy identity.
### -Name
Specifies the treatment name with `Parent`.
### -AllowedDestinations
Specifies `None`, `DomesticOnly`, `ZoneA`, or `InternationalAndDomestic`.
### -AllowedDestinationsPattern
Specifies the destination number pattern.
### -CallSource
Specifies `DialOut`, `ConferenceDialOut`, or `CallForwardSimRing`.
### -Schedule
Specifies the treatment schedule; use `$null` for `ConferenceDialOut`.
### -TimeZoneId
Specifies the schedule time zone.
### CommonParameters
This cmdlet supports the common parameters.
