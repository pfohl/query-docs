---
title: "Cube.Dimensions | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Cube.Dimensions

## Syntax

<pre>
Cube.Dimensions(**cube** as table) as table
</pre>

## About
Returns a table containing the set of available dimensions within the `cube`. Each dimension is a table containing a set of dimension attributes and each dimension attribute is represented as a column in the dimension table. Dimensions can be expanded in the cube using Cube.AddAndExpandDimensionColumn. 

