---
applicable: Microsoft Teams
author: officedocspr
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: bulenteg
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/new-csteamsdialoutpolicy
schema: 2.0.0
title: New-CsTeamsDialOutPolicy
---

# New-CsTeamsDialOutPolicy

## SYNOPSIS
Creates a Teams dial-out policy.

## SYNTAX
```
New-CsTeamsDialOutPolicy -Identity <string> [-AllowedDestinations <string>] [-AllowedDestinationsPattern <string>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Creates a policy that controls the destinations and number patterns allowed for dial-out calls.

## EXAMPLES
### Example 1
```powershell
New-CsTeamsDialOutPolicy -Identity "LobbyPhonePolicy" -AllowedDestinations "DomesticOnly" -AllowedDestinationsPattern "^\+1"
```
Creates a policy for lobby phones that permits domestic destinations matching the specified pattern.

## PARAMETERS
### -AllowedDestinations
Specifies `None`, `DomesticOnly`, `ZoneA`, or `InternationalAndDomestic`.

### -AllowedDestinationsPattern
Specifies the number pattern used to limit allowed destinations.

### -Identity
Specifies the unique identity of the new policy.

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable.

## INPUTS
### None

## OUTPUTS
### System.Object
