---
applicable: Microsoft Teams
author: officedocspr
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-help.xml
Locale: en-US
manager: bulenteg
Module Name: MicrosoftTeams
ms.author: odocspr
online version: https://learn.microsoft.com/powershell/module/microsoftteams/remove-csteamscallbarringtreatment
schema: 2.0.0
title: Remove-CsTeamsCallBarringTreatment
---
# Remove-CsTeamsCallBarringTreatment
## SYNOPSIS
Removes a Teams call barring treatment.
## SYNTAX
```
Remove-CsTeamsCallBarringTreatment -Identity <string> [-WhatIf] [-Confirm] [<CommonParameters>]
Remove-CsTeamsCallBarringTreatment -Parent <string> -Name <string> [-WhatIf] [-Confirm] [<CommonParameters>]
```
## DESCRIPTION
Removes a treatment by combined identity or by parent policy and name.
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
### None
