---
title: "COUNT Function (DAX) | Microsoft Docs"
ms.service: powerbi 

ms.date: 11/07/2018
ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# COUNT Function (DAX)
The COUNT function counts the number of cells in a column that contain numbers.  
  
## Syntax  
  
```dax
COUNT(<column>)  
```
  
#### Parameters  
  
|Term|Definition|  
|--------|--------------|  
|column|The column that contains the numbers to be counted|  
  
## Return value  
A whole number.  
  
## Remarks  
The only argument allowed to this function is a column. The COUNT function counts rows that contain the following kinds of values:  
  
-   Numbers  
  
-   Dates  

-   Strings
  
If the row contains text that cannot be translated into a number, the row is not counted.  
  
When the function finds no rows to count, it returns a blank.  When there are rows, but none of them meet the specified criteria, then the function returns 0.  
  
## Example  
The following example shows how to count the number of numeric values in the column, ShipDate.  
  
```dax
=COUNT([ShipDate])  
```

To count logical values or text, use the COUNTA or COUNTAX functions.  
  
## See Also  
[COUNT Function &#40;DAX&#41;](count-function-dax.md)  
[COUNTA Function &#40;DAX&#41;](counta-function-dax.md)  
[COUNTAX Function &#40;DAX&#41;](countax-function-dax.md)  
[COUNTX Function &#40;DAX&#41;](countx-function-dax.md)  
[Statistical Functions &#40;DAX&#41;](statistical-functions-dax.md)  
  