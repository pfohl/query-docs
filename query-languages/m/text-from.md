---
title: "Text.From | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Text.From

  
## About  
Returns the text representation of a number, date, time, datetime, datetimezone, logical, duration or binary value. If a value is null, Text.From returns null. The optional culture parameter is used to format the text value according to the given culture.  
  
## Syntax

<pre>
Text.From(value as any, optional culture as nullable text) as nullable text  
</pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|value|Value to convert.|  
|optional culture|A text value corresponding to the culture values supported on your version of Windows, such as "en-US". If the culture is not specified, the current user culture is used. For a list of culture names, see [National Language Support (NLS) API Reference](https://msdn.microsoft.com/en-us/goglobal/bb896001.aspx).|  
  
## Examples  
  
```powerquery-m
Text.From(1) equals "1"  
```  
  
```powerquery-m
Text.From(#date(2013,5,1)) equals "05/01/2013"  
```  
  
```powerquery-m 
Text.From(#date(2013,5,1),"fr-FR") equals "01/05/2013"  
```  