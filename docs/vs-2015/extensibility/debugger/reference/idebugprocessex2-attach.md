---
title: "IDebugProcessEx2::Attach | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "IDebugProcessEx2::Attach"
helpviewer_keywords: 
  - "IDebugProcessEx2::Attach method"
ms.assetid: f3334ed7-39bf-4d02-a338-36f567b9b287
caps.latest.revision: 16
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugProcessEx2::Attach
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugProcessEx2::Attach](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugprocessex2-attach).  
  
This method informs the process that a session is now debugging the process.  
  
## Syntax  
  
```cpp#  
HRESULT Attach(   
   IDebugSession2* pSession  
);  
```  
  
```csharp  
int Attach(  
   IDebugSession2 pSession  
);  
```  
  
#### Parameters  
 `pSession`  
 [in] A value that uniquely identifies the session attaching to this process.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## Remarks  
 The interface passed in `pSession` is to be treated only as a cookie, a value that uniquely identifies the session debug manager attaching to this process; none of the methods on the supplied interface are functional.  
  
## See Also  
 [IDebugProcessEx2](../../../extensibility/debugger/reference/idebugprocessex2.md)

