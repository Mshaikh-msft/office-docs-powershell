---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/grant-csteamsdialoutpolicy
schema: 2.0.0
title: Grant-CsTeamsDialOutPolicy
---
# Grant-CsTeamsDialOutPolicy
## SYNOPSIS
Assigns a Teams dial-out policy to a user.
## SYNTAX
```
Grant-CsTeamsDialOutPolicy -Identity <string> -PolicyName <string> [-WhatIf] [-Confirm] [<CommonParameters>]
```
## DESCRIPTION
Assigns a Teams dial-out policy to the specified user.
## EXAMPLES
### Example 1
```powershell
Grant-CsTeamsDialOutPolicy -Identity "user@contoso.com" -PolicyName "LobbyPhonePolicy"
```
Assigns the policy to the user.
## PARAMETERS
### -Identity
Specifies a SIP address, user principal name, or object identity.
### -PolicyName
Specifies the policy name. Set this parameter to `$null` to remove a per-user assignment.
### CommonParameters
This cmdlet supports the common parameters.
## INPUTS
### System.Object
## OUTPUTS
### System.Object
