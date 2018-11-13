---
title: "Text.EndsWith | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Text.EndsWith

  
## About  
Returns a logical value indicating whether a text value substring was found at the end of a string.  
  
## Syntax

<pre>
Text.EndsWith(string as nullable text, substring as text, optional comparer as nullable function) as nullable logical  
</pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|string|The text value to parse.|  
|substring|The string to search for.|  
|optional comparer|An optional comparer can be provided to influence the result.|  
  
## <a name="__toc360788886"></a>Remarks  
  
-   Only comparer functions created through the library (Comparer.FromCulture) are supported.  
  