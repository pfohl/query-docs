---
title: "Text.PadEnd | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Text.PadEnd

  
## About  
Returns a text value padded at the end with pad to make it at least length characters.  
  
## Syntax

<pre>
Text.PadEnd(text as nullable text, length as number, pad as nullable text) as nullable text  
</pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|text|The text to parse.|  
|length|The length to pad to.|  
|pad|The text to pad with.|  
  
## <a name="__toc360788905"></a>Remarks  
  
-   If pad is not specified, whitespace is used as pad.  
  
## Example  
  
```powerquery-m
Text.PadEnd("abc", 5, "a") equals "abcaa"  
```  