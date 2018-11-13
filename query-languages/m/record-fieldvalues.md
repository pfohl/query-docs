---
title: "Record.FieldValues | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Record.FieldValues

  
## About  
Returns a list of field values in order of the record's fields.  
  
## Syntax

<pre>
Record.FieldValues(record as record) as list  
</pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|record|The record to check.|  
  
## Example  
  
```powerquery-m  
Record.FieldValues( [CustomerID = 1, Name = "Bob", Phone = "123-4567"] ) equals {1, "Bob", "123-4567"}  
```  