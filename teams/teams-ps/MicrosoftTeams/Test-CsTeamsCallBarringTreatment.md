---
applicable: Microsoft Teams
author: Mshaikh
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/test-csteamscallbarringtreatment
schema: 2.0.0
title: Test-CsTeamsCallBarringTreatment
---
# Test-CsTeamsCallBarringTreatment
## SYNOPSIS
Tests a Teams call barring treatment.
## SYNTAX
```
Test-CsTeamsCallBarringTreatment -Identity <string> [<CommonParameters>]
Test-CsTeamsCallBarringTreatment -Parent <string> -Name <string> [<CommonParameters>]
```
## DESCRIPTION
Tests whether a call barring treatment can be resolved and used.
## PARAMETERS
### -Identity
Specifies the combined policy and treatment identity.
### -Parent
Specifies the parent policy identity.
### -Name
Specifies the treatment name with `Parent`.
### CommonParameters
This cmdlet supports the common parameters.
## INPUTS
### None
## OUTPUTS
### System.Boolean
