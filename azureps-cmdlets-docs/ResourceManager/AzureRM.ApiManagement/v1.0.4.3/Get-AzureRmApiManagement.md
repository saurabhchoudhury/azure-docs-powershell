---
external help file: Microsoft.Azure.Commands.ApiManagement.dll-Help.xml
online version: 
schema: 2.0.0
---

# Get-AzureRmApiManagement

## SYNOPSIS
Gets a list or a particular API Management Service description.

## SYNTAX

### All In Subscription (Default)
```
Get-AzureRmApiManagement
```

### All In Resource Group
```
Get-AzureRmApiManagement -ResourceGroupName <String>
```

### Specific API Management Service
```
Get-AzureRmApiManagement -ResourceGroupName <String> -Name <String>
```

## DESCRIPTION
The Get-AzureRMApiManagement cmdlet gets a list of all API Management services under subscription or specified resource group or a particular API Management.

## EXAMPLES

### Example 1: Get all API Management services
```
PS C:\>Get-AzureRmApiManagement
```

This command gets all API Management services within a subscription.

### Example 2: Get all API Management services by a specific name
```
PS C:\>Get-AzureRmApiManagement -ResourceGroupName "ContosoGroup" -Name "ContosoApi"
```

This command gets all API Management service by name.

## PARAMETERS

### -Name
Specifies the name of API Management service.

```yaml
Type: String
Parameter Sets: Specific API Management Service
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group under in which this cmdlet gets the API Management service.

```yaml
Type: String
Parameter Sets: All In Resource Group, Specific API Management Service
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Backup-AzureRmApiManagement]()

[New-AzureRmApiManagement]()

[Remove-AzureRmApiManagement]()

[Restore-AzureRmApiManagement]()

