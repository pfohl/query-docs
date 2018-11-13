---
title: "Date.Year | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Date.Year

  
## About  
Returns the year from a DateTime value.  
  
## Syntax

<pre>
Date.Year(dateTime as datetime) as nullable number  
</pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|date|The Date to retrieve the year for.|  
  
## Example  
  
```powerquery-m
Date.Year(DateTime.FromText("2011-02-19")) equals 2011  
```  