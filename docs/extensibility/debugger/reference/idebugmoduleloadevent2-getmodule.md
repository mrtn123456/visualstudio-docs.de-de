---
title: 'IDebugModuleLoadEvent2:: GetModule | Microsoft-Dokumentation'
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugModuleLoadEvent2::GetModule
helpviewer_keywords:
- IDebugModuleLoadEvent2::GetModule
ms.assetid: c86482bb-9ce5-4e63-bbe0-969b50169424
author: acangialosi
ms.author: anthc
manager: jillfra
ms.workload:
- vssdk
dev_langs:
- CPP
- CSharp
ms.openlocfilehash: b90547709e5524ce005b0598b0b8d482cfecf173
ms.sourcegitcommit: 6cfffa72af599a9d667249caaaa411bb28ea69fd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2020
ms.locfileid: "80726725"
---
# <a name="idebugmoduleloadevent2getmodule"></a>IDebugModuleLoadEvent2::GetModule
Ruft das Modul ab, das geladen oder entladen wird.

## <a name="syntax"></a>Syntax

```cpp
HRESULT GetModule( 
   IDebugModule2** pModule,
   BSTR*           pbstrDebugMessage,
   BOOL*           pbLoad
);
```

```csharp
int GetModule( 
   out IDebugModule2 pModule,
   ref string        pbstrDebugMessage,
   ref int           pbLoad
);
```

## <a name="parameters"></a>Parameter
`pModule`\
vorgenommen Gibt ein [IDebugModule2](../../../extensibility/debugger/reference/idebugmodule2.md) -Objekt zurück, das das Modul darstellt, das geladen oder entladen wird.

`pbstrDebugMessage`\
[in, out] Gibt eine optionale Meldung zurück, die dieses Ereignis beschreibt. Wenn dieser Parameter ein NULL-Wert ist, wird keine Meldung angefordert.

`pbLoad`\
[in, out] Ungleich NULL ( `TRUE` ), wenn das Modul geladen wird, und 0 (NULL `FALSE` ) (), wenn das Modul entladen wird. Wenn dieser Parameter ein NULL-Wert ist, wird kein Status angefordert.

## <a name="return-value"></a>Rückgabewert
 Wenn die Ausführung erfolgreich ist, wird `S_OK`, andernfalls ein Fehlercode zurückgegeben.

## <a name="see-also"></a>Weitere Informationen
- [IDebugModuleLoadEvent2](../../../extensibility/debugger/reference/idebugmoduleloadevent2.md)
- [IDebugModule2](../../../extensibility/debugger/reference/idebugmodule2.md)
