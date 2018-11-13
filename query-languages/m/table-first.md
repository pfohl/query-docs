---
title: "Table.First | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Table.First

  
## About  
Returns the first row from a table.  
  
## Syntax

<pre>
Table.First(table as table, optional default as any) as any  
</pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|table|The Table to check.|  
|optional default|Optional default value.|  
  
## <a name="__toc360789480"></a>Remarks  
  
-   If the table is empty, **Table.First** returns null.  
  
## Example  
  
```powerquery-m
Table.First(Table.FromRecords({  
  
    [CustomerID = 1, Name = "Bob", Phone = "123-4567"],  
  
    [CustomerID = 2, Name = "Jim", Phone = "987-6543"],  
  
    [CustomerID = 3, Name = "Paul", Phone = "543-7890"]  
  
}))  
```  
  
|Name|Value|  
|--------|---------|  
|CustomerID|1|  
|Name|Bob|  
|Phone|123-4567|  
  