---
title: "Date.IsInPreviousNWeeks | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Date.IsInPreviousNWeeks
## Syntax

<pre>
Date.IsInPreviousNWeeks(**dateTime** as any, **weeks** as number) as nullable logical
</pre>

## About
Indicates whether the given datetime value `dateTime` occurs during the previous number of weeks, as determined by the current date and time on the system. 
* `dateTime`: A `date`, `datetime`, or `datetimezone` value to be evaluated.
* `weeks`: The number of weeks.

## Example 
Determine if the week before the current system time is in the previous two weeks.

```powerquery-m
Date.IsInPreviousNWeeks(Date.AddDays(DateTime.FixedLocalNow(), -7), 2)
```

`true`
