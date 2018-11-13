---
title: "Date.IsInNextDay | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Date.IsInNextDay

## Syntax

<pre>
Date.IsInNextDay(**dateTime** as any) as nullable logical
</pre>

## About
Indicates whether the given datetime value `dateTime` occurs during the next day, as determined by the current date and time on the system. 
- `dateTime`: A `date`, `datetime`, or `datetimezone` value to be evaluated.

## Example 
Determine if the day after the current system time is in the next day.

```powerquery-mDate.IsInNextDay(Date.AddDays(DateTime.FixedLocalNow(), 1))
```

`true`
