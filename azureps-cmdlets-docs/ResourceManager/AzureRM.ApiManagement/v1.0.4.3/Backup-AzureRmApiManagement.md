---
external help file: Microsoft.Azure.Commands.ApiManagement.dll-Help.xml
online version: 
schema: 2.0.0
---

# Backup-AzureRmApiManagement

## SYNOPSIS
Backs up an API Management service.

## SYNTAX

```
Backup-AzureRmApiManagement -ResourceGroupName <String> -Name <String> -StorageContext <AzureStorageContext>
 -TargetContainerName <String> [-TargetBlobName <String>] [-PassThru]
```

## DESCRIPTION
The Backup-AzureRmApiManagement cmdlet backs up an instance of an Azure API Management service.
This cmdlet stores the backup as an Azure Storage blob.

## EXAMPLES

### Example 1: Back up an API Management service
```
PS C:\>Backup-AzureRmApiManagement -ResourceGroupName "ContosoGroup02" -Name "ContosoApi" -StorageContext $StorageContext -TargetContainerName "ContosoBackups" -TargetBlobName "ContosoBackup.apimbackup"
```

This command backs up an API Management service to a Storage blob.

## PARAMETERS

### -Name
Specifies the name of the API Management deployment that this cmdlet backs up.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Indicates that this cmdlet returns the backed up PsApiManagement object, if the operation succeeds.

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

### -ResourceGroupName
Specifies the name of the of resource group under which the API Management deployment exists.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StorageContext
Specifies a storage connection context.

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TargetBlobName
Specifies the name of the blob for the backup.
If the blob does not exist, this cmdlet creates it.
This cmdlet generates a default value based on the following pattern:

{Name}-{yyyy-MM-dd-HH-mm}.apimbackup

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

### -TargetContainerName
Specifies the name of the container of the blob for the backup.
If the container does not exist, this cmdlet creates it.

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

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmApiManagement]()

[New-AzureRmApiManagement]()

[Remove-AzureRmApiManagement]()

[Restore-AzureRmApiManagement]()

