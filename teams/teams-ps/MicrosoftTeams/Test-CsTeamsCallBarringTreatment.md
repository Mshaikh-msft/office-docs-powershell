---
applicable: Microsoft Teams
author: Mshaikh
external help file: MicrosoftTeams-help.xml
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
Evaluates dial-out policy enforcement for a user or resource account, destination number, and call scenario.
## SYNTAX
```
Test-CsTeamsCallBarringTreatment -Identity "sip:user@contoso.com" -PhoneNumber "+14255550100" -CallScenario DialOut
Test-CsTeamsCallBarringTreatment -Body $request
```
## DESCRIPTION
Evaluates dial-out eligibility for the supplied user or resource account, destination number, and call scenario at the current time. The cmdlet does not place a call. Existing eligibility checks apply; TeamsDialOutPolicy treatments require ECS enablement for the account. ConferenceDialOut excludes user-based fallback. An allowed result does not guarantee live routing success.
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
