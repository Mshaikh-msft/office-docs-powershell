---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/get-csteamsdialoutpolicy
schema: 2.0.0
title: Get-CsTeamsDialOutPolicy
---
# Get-CsTeamsDialOutPolicy
## SYNOPSIS
Retrieves Teams dial-out policies.
## SYNTAX
```
Get-CsTeamsDialOutPolicy [[-Identity] <string>] [<CommonParameters>]
```
## DESCRIPTION
Gets one or more Teams dial-out policies. If `Identity` is omitted, all policies are returned.
## EXAMPLES
### Example 1
```powershell
Get-CsTeamsDialOutPolicy -Identity "LobbyPhonePolicy"
```
Retrieves the specified policy.
## PARAMETERS
### -Identity
Specifies the identity of the policy to retrieve. Omit this parameter to retrieve all policies.
### CommonParameters
This cmdlet supports the common parameters.
## INPUTS
### None
## OUTPUTS
### System.Object
