---
title: "Type.ForRecord | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Type.ForRecord

  
## About  
Returns a Record type from a fields record.  
  
## Syntax

<pre>
Type.ForRecord(fields as record, open as logical) as type  
</pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|fields|The record to convert.|  
|open|A logical value indicating if the returned type should be an open record.|  
  
## Example  
  
```powerquery-m
Type.ForRecord(  
[  
X = [Type = type number, Optional = false],   
Y = [Type = type number, Optional = true]], true)  
equals type [ X = number, optional Y = number,...   
]  
```  