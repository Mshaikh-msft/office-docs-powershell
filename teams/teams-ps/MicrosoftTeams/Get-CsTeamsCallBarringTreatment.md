---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/get-csteamscallbarringtreatment
schema: 2.0.0
title: Get-CsTeamsCallBarringTreatment
---
# Get-CsTeamsCallBarringTreatment
## SYNOPSIS
Gets Teams call barring treatments.
## SYNTAX
```
Get-CsTeamsCallBarringTreatment -Identity <string> [<CommonParameters>]
Get-CsTeamsCallBarringTreatment -Parent <string> [-Name <string>] [<CommonParameters>]
```
## DESCRIPTION
Gets a treatment by combined identity or treatments under a parent policy.
## PARAMETERS
### -Identity
Specifies the combined policy and treatment identity.
### -Parent
Specifies the parent policy identity.
### -Name
Specifies the treatment name under `Parent`.
### CommonParameters
This cmdlet supports the common parameters.
## INPUTS
### None
## OUTPUTS
### System.Object
