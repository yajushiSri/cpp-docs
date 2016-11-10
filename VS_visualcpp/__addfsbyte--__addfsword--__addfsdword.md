---
title: "__addfsbyte, __addfsword, __addfsdword"
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
ms.assetid: 706c70df-6b52-4401-9268-2977ed8ad715
caps.latest.revision: 7
manager: ghogen
translation.priority.ht: 
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - ru-ru
  - zh-cn
  - zh-tw
translation.priority.mt: 
  - cs-cz
  - pl-pl
  - pt-br
  - tr-tr
---
# __addfsbyte, __addfsword, __addfsdword
**Microsoft Specific**  
  
 Add a value to a memory location specified by an offset relative to the beginning of the `FS` segment.  
  
## Syntax  
  
```  
void __addfsbyte(   
   unsigned long Offset,   
   unsigned char Data   
);  
void __addfsword(   
   unsigned long Offset,   
   unsigned short Data   
);  
void __addfsdword(   
   unsigned long Offset,   
   unsigned long Data   
);  
```  
  
#### Parameters  
 [in] `Offset`  
 The offset from the beginning of `FS`.  
  
 [in] `Data`  
 The value to add to the memory location.  
  
## Requirements  
  
|Intrinsic|Architecture|  
|---------------|------------------|  
|`__addfsbyte`|x86|  
|`__addfsword`|x86|  
|`__addfsdword`|x86|  
  
## Remarks  
 These routines are available only as intrinsics.  
  
## END Microsoft Specific  
  
## See Also  
 [__incfsbyte, \__incfsword, \__incfsdword](../VS_visualcpp/__incfsbyte--__incfsword--__incfsdword.md)   
 [__readfsbyte, \__readfsdword, \__readfsqword, \__readfsword](../VS_visualcpp/__readfsbyte--__readfsdword--__readfsqword--__readfsword.md)   
 [__writefsbyte, \__writefsdword, \__writefsqword, \__writefsword](../VS_visualcpp/__writefsbyte--__writefsdword--__writefsqword--__writefsword.md)   
 [Compiler Intrinsics](../VS_visualcpp/Compiler-Intrinsics.md)