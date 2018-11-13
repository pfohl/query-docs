---
title: "DateTime.FromText | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# DateTime.FromText

  
## About  
Returns a DateTime value from a set of date formats and culture value.  
  
## Syntax

<pre>
DateTime.FromText(dateTime as nullable text, optional culture as nullable text) as nullable date </pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|dateTime|The text value to convert.|  
|Culture|A text value corresponding to the culture values supported on your version of Windows, such as "en-US". If the culture is not specified, the current user culture is used. For a list of culture names, see [National Language Support (NLS) API Reference](https://msdn.microsoft.com/en-us/goglobal/bb896001.aspx).|  
  
### DateTime formats  
  
-   YYYY-MM-DDThh:mm  
  
-   YYYYMMDDThh:mm  
  
-   YYYY-MM-DDThh:mm:ss  
  
-   YYYYMMDDThh:mm:ss  
  
-   YYYY-MM-DDThh:mm:ss.nnnnnnn  
  
-   YYYYMMDDThh:mm:ss.nnnnnnn  
  
### Terms  
  
-   Y = years  
  
-   M = months  
  
-   D = days  
  
-   h = hours  
  
-   m = minutes  
  
-   s = seconds  
  
-   n = fractional seconds  
  
## Example  
  
```powerquery-m
DateTime.FromText("2010-12-31T01:30:00") equals YYYY-MM-DDThh:mm:ss  
```  