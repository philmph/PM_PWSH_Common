---
external help file:
Module Name:
online version: https://github.com/philmph/PWSH_Common_Functions/blob/main/Docs/Get-GPONotLinkedReport.md
schema: 2.0.0
---

# Get-GPONotLinkedReport

## SYNOPSIS

Checks for unlinked GPO objects.

## SYNTAX

```powershell
Get-GPONotLinkedReport [[-Domain] <String>] [<CommonParameters>]
```

## DESCRIPTION

Checks for unlinked GPO objects by creating a domain GPO XML report and parsing it.

## EXAMPLES

### EXAMPLE 1

```powershell
Get-GPONotLinkedReport

Name       CreatedTime         ModifiedTime
----       -----------         ------------
Not Linked 12.07.2019 13:43:38 12.07.2019 13:43:38
```

## PARAMETERS

### -Domain

Defines the domain to check for unlinked gpos.
Defaults to env:USERDNSDOMAIN.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: $env:USERDNSDOMAIN
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### -

## OUTPUTS

### [PSCustomObject]

## NOTES

Author: Philipp Maier

Author Git: [philmph](https://github.com/philmph)

## RELATED LINKS

[https://github.com/philmph/PWSH_Common_Functions/blob/main/Docs/Get-GPONotLinkedReport.md](https://github.com/philmph/PWSH_Common_Functions/blob/main/Docs/Get-GPONotLinkedReport.md)
