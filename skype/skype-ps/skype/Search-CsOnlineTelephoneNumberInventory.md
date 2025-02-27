---
external help file: Microsoft.Rtc.Management.Hosted.dll-help.xml 
online version: https://docs.microsoft.com/powershell/module/skype/search-csonlinetelephonenumberinventory
applicable: Skype for Business Online
title: Search-CsOnlineTelephoneNumberInventory
schema: 2.0.0
manager: bulenteg
author: tomkau
ms.author: tomkau
ms.reviewer:
---

# Search-CsOnlineTelephoneNumberInventory

## SYNOPSIS
Use the `Search-CsOnlineTelephoneNumberInventory` cmdlet to reserve a telephone numbers that are in inventory and available to be acquired.

**Note**:

As of April 30, 2022, the existing Skype for Business PowerShell cmdlets for telephone number search and related activities will be deprecated and will no longer be available for use. The new Teams PowerShell cmdlets for telephone number search and related activities are already available. For more details, see [New-CsOnlineTelephoneNumberOrder](https://docs.microsoft.com/powershell/module/teams/new-csonlinetelephonenumberorder?view=teams-ps).

## SYNTAX

```
Search-CsOnlineTelephoneNumberInventory [-Tenant <Guid>] -RegionalGroup <String>
 -CountryOrRegion <String> -Area <String> -CapitalOrMajorCity <String> -Quantity <Int32>
 [-TelephoneNumber <String>] [-AreaCode <String>] -InventoryType <String> [-DomainController <Fqdn>] [-Force]
 [<CommonParameters>]
```

## DESCRIPTION
Acquiring tenant telephone numbers is a two step process.

+12127539059 +1 (212) 753 9059

`Select-CsOnlineTelephoneNumberInventory -ReservationId 76ce711f-9da4-46d9-b81d-471172450443 -TelephoneNumbers 12127539058,12127539059 -Region NOAM -Country US -Area NY -City NY`

## EXAMPLES

### -------------------------- Example 1 --------------------------
```
Search-CsOnlineTelephoneNumberInventory -InventoryType Service -Region NOAM -Country US -Area NY -City NY -Quantity 10
```

This example reserves 10 Service type telephone numbers in New York, New York.


## PARAMETERS

### -Area
Specifies the target geographical area for the cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CapitalOrMajorCity
Specifies the target geographical city for the cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: City
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CountryOrRegion
Specifies the target country for the cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Country
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InventoryType
Specifies the target telephone number type for the cmdlet.
Acceptable values are:

"Service" for numbers assigned to conferencing support.

"Subscriber" for numbers supporting public switched telephone network (PSTN) functions.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Quantity
Specifies the quantity of telephone numbers to reserve.
The maximum value is 500.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RegionalGroup
Specifies the target geographical region for the cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Region
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AreaCode
Specifies the area code to search for telephone numbers.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DomainController
This parameter is reserved for internal Microsoft use.

```yaml
Type: Fqdn
Parameter Sets: (All)
Aliases: DC
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
The Force switch specifies whether to suppress warning and confirmation messages.
It can be useful in scripting to suppress interactive prompts.
If the Force switch isn't provided in the command, you're prompted for administrative input if required.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TelephoneNumber
Specifies either an individual telephone number to reserve, or multiple telephone numbers can be entered separated by a comma.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tenant
Specifies your tenant identifier.
To find your tenant id use the command: `Get-CsTenant | fl objectid`.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

###  
None

## OUTPUTS

###  
This cmdlets returns an Microsoft.Rtc.Management.Hosted.Bvd.Types.NumberReservationResponse object.

## NOTES

## RELATED LINKS

