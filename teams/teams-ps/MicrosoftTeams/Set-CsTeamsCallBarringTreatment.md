---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/set-csteamscallbarringtreatment
schema: 2.0.0
title: Set-CsTeamsCallBarringTreatment
---
# Set-CsTeamsCallBarringTreatment
## SYNOPSIS
Updates a Teams call barring treatment.
## SYNTAX
```
Set-CsTeamsCallBarringTreatment -Identity <string> [-AllowedDestinations <string>] [-AllowedDestinationsPattern <string>] [-CallSource <string>] [-Schedule <object>] [-TimeZoneId <string>] [<CommonParameters>]
Set-CsTeamsCallBarringTreatment -Parent <string> -Name <string> [-AllowedDestinations <string>] [-AllowedDestinationsPattern <string>] [-CallSource <string>] [-Schedule <object>] [-TimeZoneId <string>] [<CommonParameters>]
```
## DESCRIPTION
Updates a call barring treatment. `AllowedDestinations` accepts `None`, `DomesticOnly`, `ZoneA`, or `InternationalAndDomestic`; `CallSource` accepts `DialOut`, `ConferenceDialOut`, or `CallForwardSimRing`.
## PARAMETERS
### -Identity
Specifies the combined policy and treatment identity.
### -Parent
Specifies the parent policy identity.
### -Name
Specifies the treatment name with `Parent`.
### -AllowedDestinations
Specifies the allowed destination scope.
### -AllowedDestinationsPattern
Specifies the destination number pattern.
### -CallSource
Specifies the call source.
### -Schedule
Specifies the schedule; `ConferenceDialOut` requires `$null`.
### -TimeZoneId
Specifies the schedule time zone.
### CommonParameters
This cmdlet supports the common parameters.
