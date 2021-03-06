---
external help file:
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/uninstall-pnpapp
applicable: SharePoint Server 2013, SharePoint Server 2016, SharePoint Server 2019, SharePoint Online
schema: 2.0.0
---

# Uninstall-PnPApp

## SYNOPSIS
Uninstalls an available add-in from the site

## SYNTAX 

```powershell
Uninstall-PnPApp -Identity <AppMetadataPipeBind>
                 [-Scope <AppCatalogScope>]
                 [-Connection <SPOnlineConnection>]
```

## EXAMPLES

### ------------------EXAMPLE 1------------------
```powershell
Uninstall-PnPApp -Identity 99a00f6e-fb81-4dc7-8eac-e09c6f9132fe
```

This will uninstall the specified app from the current site.

### ------------------EXAMPLE 2------------------
```powershell
Uninstall-PnPApp -Identity 99a00f6e-fb81-4dc7-8eac-e09c6f9132fe -Scope Site
```

This will uninstall the specified app from the current site. Notice that the app was original installed from the site collection appcatalog.

## PARAMETERS

### -Identity
Specifies the Id of the Addin Instance

Only applicable to: SharePoint Online

```yaml
Type: AppMetadataPipeBind
Parameter Sets: (All)

Required: True
Position: 0
Accept pipeline input: True
```

### -Scope
Defines which app catalog to use. Defaults to Tenant

Only applicable to: SharePoint Online

```yaml
Type: AppCatalogScope
Parameter Sets: (All)

Required: False
Position: Named
Accept pipeline input: False
```

### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

Only applicable to: SharePoint Online

```yaml
Type: SPOnlineConnection
Parameter Sets: (All)

Required: False
Position: Named
Accept pipeline input: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)