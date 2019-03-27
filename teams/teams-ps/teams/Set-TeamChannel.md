---
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-Help.xml
Module Name: MicrosoftTeams
online version:
schema: 2.0.0
---

# Set-TeamChannel

## SYNOPSIS

Update Team channels settings.

## SYNTAX

```
Set-TeamChannel -GroupId <String> -CurrentDisplayName <String> [-NewDisplayName <String>]
 [-Description <String>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### Example 1
```
Set-TeamChannel -GroupId c58566a6-4bb4-4221-98d4-47677dbdbef6 -CurrentDisplayName TechReads -NewDisplayName "Technical Reads"
```

## PARAMETERS

### -GroupId
GroupId of the team

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

### -CurrentDisplayName
Current channel name

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

### -NewDisplayName
New Channel display name.
Names must be 50 characters or less, and can't contain the characters # % & * { } / \ : \< \> ?
+ | ' "

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

### -Description
Updated Channel description.
Channel Description Characters Limit - 1024.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable.
For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
