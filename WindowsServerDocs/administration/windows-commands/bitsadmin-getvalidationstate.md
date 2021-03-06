---
title: bitsadmin getvalidationstate
description: "Windows Commands topic for **bitsadmin getvalidationstate** - Reports the content validation state of the given file within the job. "
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: manage-windows-commands
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 6ada3f1f-9967-4262-9d22-ed641e23f516
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# bitsadmin getvalidationstate

>Applies To: Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Reports the content validation state of the given file within the job.  
  
## Syntax  
  
```  
bitsadmin /GetValidationState <Job> <file index>   
```  
  
## Parameters  
  
|Parameter|Description|  
|-------|--------|  
|Job|The job's display name or GUID|  
|File index|starts from 0|  
  
## <a name="BKMK_examples"></a>Examples  
The following example gets the content validation state of file 2 within the job named *myJob*.  
  
```  
C:\>bitsadmin /GetValidationState myJob 1  
```  
  
## additional references  
[Command-Line Syntax Key](command-line-syntax-key.md)  
  

