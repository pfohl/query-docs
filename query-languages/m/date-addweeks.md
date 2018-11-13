---
title: "Date.AddWeeks | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Date.AddWeeks

  
## About  
Returns a Date/DateTime/DateTimeZone value incremented by the number of weeks provided. Each week is defined as a duration of seven days. It also handles incrementing the month and year potions of the value as appropriate.  
  
## Syntax

<pre>   
Date.AddWeeks(dateTime, weeks as number)  
</pre> 
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|dateTime|The DateTime to add weeks to.|  
|weeks|The number of weeks to add.|  
  
## Examples  
  
```powerquery-m  
Date.AddWeeks(DateTime.FromText("2011-02-19"), 1) equals 2011-02-26  
```  
  
```powerquery-m  
Date.AddWeeks(DateTime.FromText("2011-02-19"), -2) equals 2011-02-05  
```  
  
```powerquery-m 
Date.AddWeeks(DateTime.FromText("2011-12-31"), 1) equals 2012-01-07  
```  