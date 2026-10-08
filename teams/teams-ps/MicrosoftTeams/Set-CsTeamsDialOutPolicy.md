---
applicable: Microsoft Teams
author: officedocspr
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: bulenteg
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/set-csteamsdialoutpolicy
schema: 2.0.0
title: Set-CsTeamsDialOutPolicy
---
# Set-CsTeamsDialOutPolicy
## SYNOPSIS
Updates a Teams dial-out policy.
## SYNTAX
```
Set-CsTeamsDialOutPolicy -Identity <string> [-AllowedDestinations <string>] [-AllowedDestinationsPattern <string>] [-WhatIf] [-Confirm] [<CommonParameters>]
```
## DESCRIPTION
Changes the destination scope or number pattern of an existing Teams dial-out policy.
## EXAMPLES
### Example 1
```powershell
Set-CsTeamsDialOutPolicy -Identity "LobbyPhonePolicy" -AllowedDestinations "InternationalAndDomestic" -AllowedDestinationsPattern "^\+"
```
Updates the policy for lobby phones.
## PARAMETERS
### -AllowedDestinations
Specifies `None`, `DomesticOnly`, `ZoneA`, or `InternationalAndDomestic`.
### -AllowedDestinationsPattern
Specifies the number pattern used to limit allowed destinations.
### -Identity
Specifies the identity of the policy to update.
### CommonParameters
This cmdlet supports the common parameters.
## INPUTS
### None
## OUTPUTS
### System.Object
