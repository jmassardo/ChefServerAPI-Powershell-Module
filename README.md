# Chef Server PowerShell Module

> WARNING. WORK IN PROGRESS. DO NOT USE IN PRODUCTION!!!

This repo contains a PowerShell module for interacting with the Chef Server.

## Configuration

Oped the `ChefServerAPI-Module.psd1` and edit the following lines:

``` powershell
OrgRootURL = "https://chef-server.example.com"
OrgName = "lab"
ChefUserPem = "admin.pem"
```

## Usage

To use, first import the module:

``` powershell
Import-Module ./ChefServerAPI-Module.psm1
```

To view the available options:

```powershell
Get-Command -Module ChefServerAPI-Module
```

Example usage:

```powershell
Get-ChefNodes
```

To uninstall:

```powershell
Remove-Module ChefServerAPI-Module
```
