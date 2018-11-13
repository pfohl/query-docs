---
title: "PATHCONTAINS Function (DAX) | Microsoft Docs"
ms.service: powerbi 

ms.date: 11/07/2018
ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# PATHCONTAINS Function (DAX)
Returns **TRUE** if the specified *item* exists within the specified *path*.  
  
## Syntax  
  
```dax
PATHCONTAINS(<path>, <item>)  
```
  
#### Parameters  
path  
A string created as the result of evaluating a PATH function.  
  
item  
A text expression to look for in the path result.  
  
## Return value  
A value of **TRUE** if *item* exists in *path*; otherwise **FALSE**.  
  
## Remarks  
If *item* is an integer number it is converted to text and then the function is evaluated. If conversion fails then the function returns an error.  
  
This DAX function is not supported for use in DirectQuery mode. For more information about limitations in DirectQuery models, see  [https://go.microsoft.com/fwlink/?LinkId=219172](https://go.microsoft.com/fwlink/?LinkId=219172).  
  
## Example  
The following example creates a calculated column that takes a manager ID and checks a set of employees. If the manager ID is among the list of managers returned by the PATH function, the PATHCONTAINS function returns true; otherwise it returns false.  
  
```dax
=PATHCONTAINS(PATH(Employee[EmployeeKey], Employee[ParentEmployeeKey]), "23")  
```