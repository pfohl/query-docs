---
title: "Text.Repeat | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Text.Repeat

  
## About  
Returns a text value composed of the input text value repeated a number of times.  
  
## Syntax

<pre>
Text.Repeat(string as text, repeatCount as number) as text  
</pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|string|The text to repeat.|  
|repeatCount|The number of times to repeat the text.|  
  
## Example  
  
```powerquery-m
Text.Repeat("a",5) equals "aaaaa"  
```  