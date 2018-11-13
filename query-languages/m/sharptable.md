---
title: "#table | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# #table

## Syntax

<pre>
#table(<b>columns</b> as any, <b>rows</b> as any) as any
</pre>

## About
Creates a table value from columns `columns` and the list `rows` where each element of the list is an inner list that contains the column values for a single row. `columns` may be a list of column names, a table type, a number of columns, or null.

  