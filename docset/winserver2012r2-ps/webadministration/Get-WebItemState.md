---
external help file: Microsoft.IIS.PowerShell.Provider.dll-Help.xml
Module Name: WebAdministration
online version: 
schema: 2.0.0
title: Get-WebItemState
description: 
keywords: powershell, cmdlet
author: andreabarr
manager: jasgro
ms.date: 2017-10-30
ms.topic: reference
ms.prod: powershell
ms.technology: powershell
ms.assetid: 9723EF9F-657A-4450-9CB9-06A93E628370
ms.author: v-anbarr
ms.reviewer: brianlic
---

# Get-WebItemState

## SYNOPSIS
Gets the run-time state of a site or an application pool.

## SYNTAX

```
Get-WebItemState [-Protocol <String>] [[-PSPath] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-WebItemState** cmdlet gets the run-time state of a site or an application pool.

## EXAMPLES

### Example 1: Get the state of all websites
```
C:\PS>Get-WebItemState -PSPath "IIS:\sites\*"
```

This command returns information about the state of all the sites on the IIS server.

### Example 2: Get the state of the default website using HTTP
```
IIS:\>Get-WebItemState -PSPath '.\Default Web Site' -Protocol "http"

Value

-----

Started
```

This command returns information about the HTTP binding on the default website.

## PARAMETERS

### -PSPath
Specifies the path to the application pool or site.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Protocol
Specifies the protocol binding for which information is returned, such as HTTP or FTP.
This parameter is for sites only.

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### PSObject

## OUTPUTS

### PSObject

## NOTES

## RELATED LINKS

