---
applicable: Microsoft Teams
author: Mshaikh
external help file: MicrosoftTeams-help.xml
Locale: en-US
manager: Roykuntz
Module Name: MicrosoftTeams
ms.author: Mshaikh
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
Specifies the object ID or SIP address of a user or resource account in the administered tenant. The `sip:` prefix is optional. A UPN works only when it matches the SIP address.
### -PhoneNumber
Specifies the destination phone number to evaluate, in E.164 format.
### -CallScenario
Specifies the call scenario to evaluate, such as `DialOut`.
### -Body
Specifies a request object containing the identity, phone number, and call scenario. Use this parameter set instead of supplying the values individually.
### CommonParameters
This cmdlet supports the common parameters.
## INPUTS
### None
## OUTPUTS
### Microsoft.Teams.ConfigAPI.Cmdlets.Generated.Models.TestTeamsCallBarringTreatmentResponse
Returns `IsBlocked`, `TreatmentName`, and `Reason`. `TreatmentName` is null unless a TeamsDialOutPolicy treatment blocks the scenario. `Reason` is null when allowed.
