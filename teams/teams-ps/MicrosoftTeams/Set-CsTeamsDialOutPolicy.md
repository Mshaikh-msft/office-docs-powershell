---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: mshaikh
online version: https://learn.microsoft.com/powershell/module/microsoftteams/set-csteamsdialoutpolicy
schema: 2.0.0
title: Set-CsTeamsDialOutPolicy
---
# Set-CsTeamsDialOutPolicy
## SYNOPSIS
Updates a Teams dial-out policy.
## SYNTAX
```
Set-CsTeamsDialOutPolicy -Identity <string> [-CallBarringTreatments <Object>] [-Description <string>] [-WhatIf] [-Confirm] [<CommonParameters>]
```
## DESCRIPTION
Updates the call barring treatments and description of an existing Teams dial-out policy.
## EXAMPLES
### Example 1
```powershell
Set-CsTeamsDialOutPolicy -Identity "LobbyPhonePolicy" -Description "Updated dial-out policy for lobby phones"
```
Updates the description of the policy for lobby phones.
## PARAMETERS
### -CallBarringTreatments
Specifies the call barring treatments associated with the policy.
### -Description
Specifies a description for the policy.
### -Identity
Specifies the identity of the policy to update.
### CommonParameters
This cmdlet supports the common parameters.
## INPUTS
### None
## OUTPUTS
### None
