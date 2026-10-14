---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
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
New-CsTeamsDialOutPolicy -Identity <string> [-CallBarringTreatments <Object>] [-Description <string>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Creates a Teams dial-out policy that can be configured with call barring treatments.

## EXAMPLES
### Example 1
```powershell
New-CsTeamsDialOutPolicy -Identity "LobbyPhonePolicy" -Description "Dial-out policy for lobby phones"
New-CsTeamsCallBarringTreatment -Parent "LobbyPhonePolicy" -Name "DomesticOnly" -AllowedDestinations "DomesticOnly" -AllowedDestinationsPattern "^\+1" -CallSource "DialOut"
```
Creates a policy for lobby phones, then configures a treatment that permits domestic destinations matching the specified pattern.

## PARAMETERS
### -CallBarringTreatments
Specifies the call barring treatments associated with the policy.

### -Description
Specifies a description for the policy.

### -Identity
Specifies the unique identity of the new policy.

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable.

## INPUTS
### None

## OUTPUTS
### System.Object
