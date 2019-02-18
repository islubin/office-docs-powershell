---
external help file: Microsoft.SharePoint.PowerShell.dll-help.xml
applicable: SharePoint Server 2019
title: Set-SPApplicationCredentialKey
schema: 2.0.0
---

# Set-SPApplicationCredentialKey

## SYNOPSIS
Sets the application credential key on the local server.


## SYNTAX

```
Set-SPApplicationCredentialKey [-Password] <SecureString> [-AssignmentCollection <SPAssignmentCollection>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```


## DESCRIPTION
Use the **Set-SPApplicationCredentialKey** cmdlet to set the application credential key on the local server, which is used by certain features to encrypt and decrypt passwords.

The application credential key must be identical on each server in the farm where it is set.

## EXAMPLES

### EXAMPLE 
```powershell
 $key = ConvertTo-SecureString -String "New Password" -AsPlainText -Force
Set-SPApplicationCredentialKey -Password $key
```

This example sets the application credential key on the local server to "New Password".

## PARAMETERS

### -Password
Specifies the application credential key.
Avoid reusing the farm passphrase or service account passwords for the application credential key.

```yaml
Type: SecureString
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Server 2019
Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -AssignmentCollection
Manages objects for the purpose of proper disposal.
Use of objects, such as SPWeb or SPSite, can use large amounts of memory and use of these objects in Windows PowerShell scripts requires proper memory management.
Using the SPAssignment object, you can assign objects to a variable and dispose of the objects after they are needed to free up memory.
When SPWeb, SPSite, or SPSiteAdministration objects are used, the objects are automatically disposed of if an assignment collection or the Global parameter is not used.

When the Global parameter is used, all objects are contained in the global store.
If objects are not immediately used, or disposed of by using the Stop-SPAssignment command, an out-of-memory scenario can occur.

```yaml
Type: SPAssignmentCollection
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Server 2010, SharePoint Server 2013, SharePoint Server 2016, SharePoint Server 2019
Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```
### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf
Applicable: SharePoint Server 2010, SharePoint Server 2013, SharePoint Server 2016, SharePoint Server 2019
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
Applicable: SharePoint Server 2010, SharePoint Server 2013, SharePoint Server 2016, SharePoint Server 2019
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable.
For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/?LinkID=113216).


## RELATED LINKS
[Remove-SPApplicationCredentialKey](Remove-SPApplicationCredentialKey.md)


