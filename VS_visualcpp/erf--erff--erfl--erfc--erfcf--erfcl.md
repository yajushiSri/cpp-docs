---
title: "erf, erff, erfl, erfc, erfcf, erfcl"
ms.custom: na
ms.date: 10/03/2016
ms.devlang: 
  - C++
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-cpp
ms.tgt_pltfrm: na
ms.topic: article
apiname: 
  - erff
  - erfl
  - erf
apilocation: 
  - msvcrt.dll
  - msvcr80.dll
  - msvcr90.dll
  - msvcr100.dll
  - msvcr100_clr0400.dll
  - msvcr110.dll
  - msvcr110_clr0400.dll
  - msvcr120.dll
  - msvcr120_clr0400.dll
  - ucrtbase.dll
  - api-ms-win-crt-math-l1-1-0.dll
apitype: DLLExport
ms.assetid: 144d90d3-e437-41c2-a659-cd57596023b5
caps.latest.revision: 7
manager: ghogen
translation.priority.ht: 
  - cs-cz
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - pl-pl
  - pt-br
  - ru-ru
  - tr-tr
  - zh-cn
  - zh-tw
---
# erf, erff, erfl, erfc, erfcf, erfcl
Computes the error function or the complementary error function of a value.  
  
## Syntax  
  
```  
double erf(  
   double x  
);  
float erf(  
   float x  
); // C++ only  
long double erf(  
   long double x  
); // C++ only  
float erff(  
   float x  
);  
long double erfl(  
   long double x  
);  
double erfc(  
   double x  
);  
float erfc(  
   float x  
); // C++ only  
long double erfc(  
   long double x  
); // C++ only  
float erfcf(  
   float x  
);  
long double erfcl(  
   long double x  
);  
```  
  
#### Parameters  
 `x`  
 A floating-point value.  
  
## Return Value  
 The `erf` functions return the Gauss error function of `x`. The `erfc` functions return the complementary Gauss error function of `x`.  
  
## Remarks  
 The `erf` functions calculate the Gauss error function of x, which is defined as:  
  
 ![The error function of x](../VS_visualcpp/media/CRT_erf_formula.PNG "CRT_erf_formula")  
  
 The complementary Gauss error function is defined as 1 – erf(x). The `erf` functions return a value in the range -1.0 to 1.0. There is no error return. The `erfc` functions return a value in the range 0 to 2. If `x` is too large for `erfc`, the `errno` variable is set to `ERANGE`.  
  
 Because C++ allows overloading, you can call overloads of `erf` and `erfc` that take and return `float` and `long double` types. In a C program, `erf` and `erfc` always take and return a `double`.  
  
## Requirements  
  
|Function|Required header|  
|--------------|---------------------|  
|`erf`, `erff`, `erfl`, `erfc`, `erfcf`, `erfcl`|<math.h>|  
  
 For additional compatibility information, see [Compatibility](../VS_visualcpp/Compatibility.md).  
  
## .NET Framework Equivalent  
 Not applicable. To call the standard C function, use `PInvoke`. For more information, see [Platform Invoke Examples](../Topic/Platform%20Invoke%20Examples.md).  
  
## See Also  
 [Floating-Point Support](../VS_visualcpp/Floating-Point-Support.md)