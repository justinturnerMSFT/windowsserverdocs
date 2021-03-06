---
title: Using the remove-DriverGroupFilter Command
description: "Windows Commands topic for **** - "
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: manage-windows-commands
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 837bd5d4-c79d-4714-942d-9875bd8e61dc
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# Using the remove-DriverGroupFilter Command

>Applies To: Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

removes a filter rule from a driver group on a server.
## Syntax
```
wdsutil /remove-DriverGroupFilter /DriverGroup:<Group Name> [/Server:<Server name>] /Filtertype:<Filter type>
```
## Parameters
|Parameter|Description|
|-------|--------|
|/DriverGroup:<Group Name>|Specifies the name of the driver group.|
|[/Server:<Server name>]|Specifies the name of the server. This can be the NetBIOS name or the FQDN. If a server name is not specified, the local server is used.|
|[/Filtertype:<Filtertype>]|Specifies the type of the filter to remove from the group. <Filtertype> can be one of the following:<br /><br />**BiosVendor**<br /><br />**Biosversion**<br /><br />**Chassistype**<br /><br />**Manufacturer**<br /><br />**Uuid**<br /><br />**Osversion**<br /><br />**Osedition**<br /><br />**OsLanguage**|
## <a name="BKMK_examples"></a>Examples
To remove a filter, type one of the following:
```
wdsutil /remove-DriverGroupFilter /DriverGroup:printerdrivers /Filtertype:Manufacturer
```
```
wdsutil /remove-DriverGroupFilter /DriverGroup:printerdrivers /Filtertype:Manufacturer /Filtertype:OSLanguage
```
#### additional references
[Command-Line Syntax Key](command-line-syntax-key.md)
