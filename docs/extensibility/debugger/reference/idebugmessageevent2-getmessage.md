---
title: 'IDebugMessageEvent2:: getMessage | Microsoft-Dokumentation'
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugMessageEvent2::GetMessage
helpviewer_keywords:
- GetMessage method
- IDebugMessageEvent2::GetMessage method
ms.assetid: 9fca7285-f7f1-422d-8565-92bf0e0db60a
author: acangialosi
ms.author: anthc
manager: jillfra
ms.workload:
- vssdk
dev_langs:
- CPP
- CSharp
ms.openlocfilehash: 819b796a656f0ef8775fbb1c9e800e3019b81729
ms.sourcegitcommit: 6cfffa72af599a9d667249caaaa411bb28ea69fd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2020
ms.locfileid: "80727400"
---
# <a name="idebugmessageevent2getmessage"></a>IDebugMessageEvent2::GetMessage
Ruft die Meldung ab, die angezeigt werden soll.

## <a name="syntax"></a>Syntax

```cpp
HRESULT GetMessage( 
   MESSAGETYPE* pMessageType,
   BSTR*        pbstrMessage,
   DWORD*       pdwType,
   BSTR*        pbstrHelpFileName,
   DWORD*       pdwHelpId
);
```

```csharp
int GetMessage( 
   out enum_MESSAGETYPE pMessageType,
   out string           pbstrMessage,
   out uint             pdwType,
   out string           pbstrHelpFileName,
   out uint             dwHelpId
);
```

## <a name="parameters"></a>Parameter
`pMessageType`\
vorgenommen Gibt einen Wert aus der [MessageType](../../../extensibility/debugger/reference/messagetype.md) -Enumeration zurück, der den Typ der Nachricht beschreibt.

`pbstrMessage`\
vorgenommen Gibt die Nachricht zurück.

`pdwType`\
vorgenommen Gibt den Typ der Nachricht zurück, wobei die Konventionen der Win32- `MessageBox` Funktion verwendet werden. Ausführliche Informationen finden Sie in der [AfxMessageBox](/cpp/mfc/reference/cstring-formatting-and-message-box-display#afxmessagebox) -Funktion.

`pbstrHelpFileName`\
[in, out] Gibt den Namen der Hilfedatei zurück. Kann ein NULL-Wert (C++) oder ein leerer Wert (c#) sein, wenn keine Hilfedatei vorhanden ist.

`pdwHelpId`\
[in, out] Gibt den Hilfe Bezeichner zurück. Kann 0 sein, wenn dieser Nachricht keine Hilfe zugeordnet ist.

## <a name="return-value"></a>Rückgabewert
 Wenn die Ausführung erfolgreich ist, wird `S_OK`, andernfalls ein Fehlercode zurückgegeben.

## <a name="see-also"></a>Weitere Informationen
- [IDebugMessageEvent2](../../../extensibility/debugger/reference/idebugmessageevent2.md)
- [MESSAGETYPE](../../../extensibility/debugger/reference/messagetype.md)
- [AfxMessageBox](/cpp/mfc/reference/cstring-formatting-and-message-box-display#afxmessagebox)
