---
title: "List.Distinct | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# List.Distinct

  
## About  
Filters a list down by removing duplicates. An optional equation criteria value can be specified to control equality comparison.  The first value from each equality group is chosen.  
  
For more information about equationCriteria, see Parameter Values.  
  
## Syntax

<pre>
List.Distinct(list as list, optional equationCriteria as any, criteria as any) as list  
</pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|list|The List to check.|  
|optional equationCriteria|An equality group equation.|  
|criteria|Filter criteria.|  
  
## Examples  
  
```powerquery-m
List.Distinct({1, 2, 3, 2, 3}) equals {1, 2, 3}  
```  
  
```powerquery-m
List.Distinct({"a","b","A"}, each _) equals {"a", "b", "A"}  
```  
  
```powerquery-m
List.Distinct({"a","b","A"}, Comparer.FromCulture("en",true)) equals {"a", "b"}  
```  
  
```powerquery-m
List.Distint({[a="a",b=2],[a="b",b=3],[a="A",b=4]},   
{ each [a] , Comparer.FromCulture("en", true) } )   
equals { [ a = "a", b = 2 ],   
//   [a = "b",  b = 3 ] }  
```  