---
title: "LN Function (DAX) | Microsoft Docs"
ms.service: powerbi 

ms.date: 11/07/2018
ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# LN Function (DAX)
Returns the natural logarithm of a number. Natural logarithms are based on the constant e (2.71828182845904).  
  
## Syntax  
  
```dax
LN(<number>)  
```
  
#### Parameters  
  
|Term|Definition|  
|--------|--------------|  
|number|The positive number for which you want the natural logarithm.|  
  
## Return value  
A decimal number.  
  
## Remarks  
LN is the inverse of the EXP function.  
  
## Example  
The following example returns the natural logarithm of the number in the column, `[Values]`.  
  
```dax
=LN([Values])  
```
  
## See Also  
[Math and Trig Functions &#40;DAX&#41;](math-and-trig-functions-dax.md)  
[EXP Function &#40;DAX&#41;](exp-function-dax.md)  
  