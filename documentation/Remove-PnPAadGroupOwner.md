---
Module Name: PnP.PowerShell
title: Remove-PnPAadGroupOwner
schema: 2.0.0
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
online version: https://pnp.github.io/powershell/cmdlets/Remove-PnPAadGroupOwner.html
---
 
# Remove-PnPAadGroupOwner

## SYNOPSIS

**Required Permissions**

  * Microsoft Graph API : One of Directory.ReadWrite.All, Group.ReadWrite.All

Removes owners from a particular Azure Active Directory group. This can be a security, distribution or Microsoft 365 group.

## SYNTAX

```powershell
Remove-PnPAadGroupOwner -Identity <AadGroupPipeBind> -Users <String[]>
  [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Remove-PnPAadGroupOwner -Identity "Project Team" -Users "john@contoso.onmicrosoft.com","jane@contoso.onmicrosoft.com"
```

Removes the provided two users as owners from the Azure Active Directory group named "Project Team"

## PARAMETERS

### -Identity
The Identity of the zure Active Directory group to remove owners from

```yaml
Type: AadGroupPipeBind
Parameter Sets: (All)

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Users
The UPN(s) of the user(s) to remove as owners from the Azure Active Directory group

```yaml
Type: String[]
Parameter Sets: (All)

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## RELATED LINKS

[Microsoft 365 Patterns and Practices](https://aka.ms/m365pnp)[Documentation](https://docs.microsoft.com/graph/api/group-delete-owners)