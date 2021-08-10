---
external help file:
Module Name:
online version: https://github.com/philmph/PWSH_Common_Functions/blob/main/Docs/Get-ADDirectoryServerOperationMasterRole.md
schema: 2.0.0
---

# Get-ADDirectoryServerOperationMasterRole

## SYNOPSIS

Used to query fsmo owners.

## SYNTAX

```powershell
Get-ADDirectoryServerOperationMasterRole [[-DomainName] <String[]>] [<CommonParameters>]
```

## DESCRIPTION

Used to query one or more domains for their fsmo owners.

## EXAMPLES

### EXAMPLE 1
```powershell
Get-ADDirectoryServerOperationMasterRole -DomainName 'pmaier.lab'

DomainName           : pmaier.lab
DomainNamingMaster   : WIN-5LI9IQMANGJ.pmaier.lab
SchemaMaster         : WIN-5LI9IQMANGJ.pmaier.lab
InfrastructureMaster : WIN-5LI9IQMANGJ.pmaier.lab
PDCEmulator          : WIN-5LI9IQMANGJ.pmaier.lab
RIDMaster            : WIN-5LI9IQMANGJ.pmaier.lab
```

### EXAMPLE 2

```powershell
'pmaier.lab' | Get-ADDirectoryServerOperationMasterRole

DomainName           : pmaier.lab
DomainNamingMaster   : WIN-5LI9IQMANGJ.pmaier.lab
SchemaMaster         : WIN-5LI9IQMANGJ.pmaier.lab
InfrastructureMaster : WIN-5LI9IQMANGJ.pmaier.lab
PDCEmulator          : WIN-5LI9IQMANGJ.pmaier.lab
RIDMaster            : WIN-5LI9IQMANGJ.pmaier.lab
```

## PARAMETERS

### -DomainName

Defines one or more domainnames to query for fsmo owners.
Defaults to env:USERDNSDOMAIN.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: $env:USERDNSDOMAIN
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### [System.String]

## OUTPUTS

### [PSCustomObject]

## NOTES

Author: Philipp Maier

Author Git: [philmph](https://github.com/philmph)

## RELATED LINKS

[https://github.com/philmph/PWSH_Common_Functions/blob/main/Docs/Get-ADDirectoryServerOperationMasterRole.md](https://github.com/philmph/PWSH_Common_Functions/blob/main/Docs/Get-ADDirectoryServerOperationMasterRole.md)
