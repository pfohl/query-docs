---
title: "Date.AddDays | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Date.AddDays

  
## About  
Returns a Date/DateTime/DateTimeZone value with the day portion incremented by the number of days provided. It also handles incrementing the month and year potions of the value as appropriate.  
  
## Syntax

<pre>   
Date.AddDays(dateTime, days as number)  
</pre> 
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|dateTime|The DateTime to add days to.|  
|days|The number of days to add.|  
  
## Examples  
  
```powerquery-m  
Date.AddDays(DateTime.FromText("2011-02-19"), 5) equals 2011-02-24  
```  
  
```powerquery-m  
Date.AddDays(DateTime.FromText("2011-02-19"), -2) equals 2011-02-17  
```  
  
```powerquery-m 
Date.AddDays(DateTime.FromText("2011-12-31"), 1) equals 2012-01-01  
```  