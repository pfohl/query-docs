---
title: "RowExpression.Column | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# RowExpression.Column

## Syntax

<pre>
RowExpression.Column(columnName as text) as record  
</pre>
  
## About  
Returns an AST that represents access to column columnName of the row within a row expression.  
  
### Example 1  
Creates an AST representing access of column "CustomerName".  
  
```powerquery-m
RowExpression.Column("CustomerName")  
```  