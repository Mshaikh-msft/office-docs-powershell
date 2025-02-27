---
external help file: Microsoft.Rtc.Management.Hosted.dll-help.xml
online version: https://docs.microsoft.com/powershell/module/skype/export-csonlineaudiofile
applicable: Microsoft Teams
title: Export-CsOnlineAudioFile
schema: 2.0.0
manager: bulenteg
author: jenstrier
ms.author: jenstr
ms.reviewer:
---

# Export-CsOnlineAudioFile

## SYNOPSIS
Use the Export-CsOnlineAudioFile cmdlet to download an existing audio file.

## SYNTAX

```powershell
Export-CsOnlineAudioFile [[-Identity] <string>] [-ApplicationId] <OrgAutoAttendant|HuntGroup|TenantGlobal>] [<CommonParameters>]
```


## DESCRIPTION
The Export-CsOnlineAudioFile cmdlet downloads an existing Auto Attendant (AA), Call Queue (CQ) service or Music on Hold audio file.


## EXAMPLES

### -------------------------- Example 1 --------------------------
```powershell
$content=Export-CsOnlineAudioFile -ApplicationId "HuntGroup" -Identity 57f800408f8848548dd1fbc18073fe46
[System.IO.File]::WriteAllBytes('C:\MyWaveFile.wav', $content)
```

This example exports a Call Queue audio file and saves it as MyWaveFile.wav.

## PARAMETERS

### -ApplicationId
The ApplicationId parameter is the identifier for the application which will use this audio file. For example, if the audio file is used with an organizational auto attendant, then it needs to be set to "OrgAutoAttendant". If the audio file is used with a hunt group (call queue), then it needs to be set to "HuntGroup". If the audio file is used with Microsoft Teams, then it needs to be set to "TenantGlobal"

Supported values:

- OrgAutoAttendant
- HuntGroup
- TenantGlobal

```yaml
Type: System.string
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams

Required: True
Position: Named
Default value: TenantGlobal
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
The Id of the specific audio file that you would like to export.


```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### None

## OUTPUTS

### Byte[]

## NOTES
You are responsible for independently clearing and securing all necessary rights and permissions to use any music or audio file with your Microsoft Teams service, which may include intellectual property and other rights in any music, sound effects, audio, brands, names, and other content in the audio file from all relevant rights holders, which may include artists, actors, performers, musicians, songwriters, composers, record labels, music publishers, unions, guilds, rights societies, collective management organizations and any other parties who own, control or license the music copyrights, sound effects, audio and other intellectual property rights.

## RELATED LINKS
[Get-CsOnlineAudioFile](Get-CsOnlineAudioFile.md)

[Import-CsOnlineAudioFile](Import-CsOnlineAudioFile.md)

[Remove-CsOnlineAudioFile](Remove-CsOnlineAudioFile.md)
