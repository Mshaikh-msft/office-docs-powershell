---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/remove-csteamsdialoutpolicy
schema: 2.0.0
title: Remove-CsTeamsDialOutPolicy
---
# Remove-CsTeamsDialOutPolicy
## SYNOPSIS
Removes a Teams dial-out policy.
## SYNTAX
```
Remove-CsTeamsDialOutPolicy -Identity <string> [-WhatIf] [-Confirm] [<CommonParameters>]
```
## DESCRIPTION
Deletes an existing Teams dial-out policy.
## EXAMPLES
### Example 1
```powershell
Remove-CsTeamsDialOutPolicy -Identity "LobbyPhonePolicy"
```
Removes the specified policy.
## PARAMETERS
### -Identity
Specifies the identity of the policy to remove.
### CommonParameters
This cmdlet supports the common parameters.
## INPUTS
### None
## OUTPUTS
### None
