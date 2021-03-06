---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
---

# New-AzureRMTenantSubscription

## SYNOPSIS
Creates a subscription as a tenant for the specified offer.

## SYNTAX

```
New-AzureRMTenantSubscription -OfferId <String> [-DisplayName <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRMTenantSubscription** cmdlet creates a subscription as a tenant for the specified offer.

## EXAMPLES

### Example 1:
```
$Offer =  Get-AzureRMOffer -Provider "default" | Where-Object name -eq "ComputeOffer"
New-AzureRmTenantSubscription  -OfferId $offer.Id -DisplayName "Compute Subscription"
```

This example creates a subscription for the logged-in tenant user.

## PARAMETERS

### -DisplayName
Specifies the name of the tenant subscription.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
Not specified.

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa
Accepted values: SilentlyContinue, Stop, Continue, Inquire

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Not specified.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OfferId
Specifies the ID of the offer to which the tenant is subscribing.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PipelineVariable
Not specified.

```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Microsoft.AzureStack.Management.Models.SubscriptionDefinition

## NOTES

## RELATED LINKS
