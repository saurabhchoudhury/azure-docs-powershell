---
external help file: Microsoft.Azure.Commands.Sql.dll-Help.xml
online version: 
schema: 2.0.0
---

# Remove-AzureRmSqlServerThreatDetectionPolicy

## SYNOPSIS
Removes the threat detection policy from a server.

## SYNTAX

```
Remove-AzureRmSqlServerThreatDetectionPolicy [-PassThru] [-ServerName] <String> [-ResourceGroupName] <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## DESCRIPTION
The Remove-AzureRmSqlServerThreatDetectionPolicy cmdlet removes the threat detection policy from an Azure SQL server.

To use this cmdlet, specify the ResourceGroupName and ServerName parameters to identify the server from which this cmdlet removes the policy.

## EXAMPLES

### --------------------------  Example 1: Remove a threat detection policy for a database  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\> Remove-AzureRmSqlServerThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

This command removes the threat detection policy from a server named Server01.

## PARAMETERS

### -PassThru
Returns an object representing the item with which you are working.
By default, this cmdlet does not generate any output.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServerName
Specifies the name of a server.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group the server is assigned to.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### 
You cannot pipe input to this cmdlet.

## OUTPUTS

### Microsoft.Azure.Commands.Sql.ThreatDetection.Model.ServerThreatDetectionPolicyModel
This cmdlet returns a ServerThreatDetectionPolicyModel object.

## NOTES

## RELATED LINKS

[Get-AzureRmSqlServerThreatDetectionPolicy]()

[Set-AzureRmSqlServerThreatDetectionPolicy]()

