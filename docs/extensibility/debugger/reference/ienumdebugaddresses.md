---
title: Ienumdebug-Adressen | Microsoft-Dokumentation
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IEnumDebugAddresses
helpviewer_keywords:
- IEnumDebugAddresses interface
ms.assetid: 5f6f6751-e6d8-4c5a-8e81-414b6e5d8cc5
author: acangialosi
ms.author: anthc
manager: jillfra
ms.workload:
- vssdk
ms.openlocfilehash: 14b42ec37babe72b47b0e832397d33029c4fc3d1
ms.sourcegitcommit: 6cfffa72af599a9d667249caaaa411bb28ea69fd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2020
ms.locfileid: "80717585"
---
# <a name="ienumdebugaddresses"></a>IEnumDebugAddresses
Diese Schnittstelle stellt eine Auflistung von Objekten dar, die die [idebugaddress](../../../extensibility/debugger/reference/idebugaddress.md) -Schnittstelle implementieren.

## <a name="syntax"></a>Syntax

```
IEnumDebugAdresses : IUnknown
```

## <a name="notes-for-implementers"></a>Hinweise für Implementierer
 Diese Schnittstelle wird vom Symbol Anbieter implementiert, um Sätze von Objekten bereitzustellen, die die [idebugaddress](../../../extensibility/debugger/reference/idebugaddress.md) -Schnittstelle implementieren. Beachten Sie, dass es sich hierbei nicht um eine com-Standard Enumeration handelt, da die [GetCount](../../../extensibility/debugger/reference/ienumdebugaddresses-getcount.md) -Methode vorhanden ist.

## <a name="notes-for-callers"></a>Hinweise für Aufrufer
 Diese Schnittstelle wird von [getaddressesfromcontext](../../../extensibility/debugger/reference/idebugsymbolprovider-getaddressesfromcontext.md) und [getaddressesfromposition](../../../extensibility/debugger/reference/idebugsymbolprovider-getaddressesfromposition.md)zurückgegeben.

## <a name="methods-in-vtable-order"></a>Methoden in der Vtable-Reihenfolge
 Diese Schnittstelle implementiert die folgenden Methoden.

|Methode|BESCHREIBUNG|
|------------|-----------------|
|[Nächste](../../../extensibility/debugger/reference/ienumdebugaddresses-next.md)|Ruft den nächsten Satz von [idebugaddress](../../../extensibility/debugger/reference/idebugaddress.md) -Objekten aus der-Enumeration ab.|
|[Skip](../../../extensibility/debugger/reference/ienumdebugaddresses-skip.md)|Überspringt eine angegebene Anzahl von Einträgen.|
|[Zurücksetzen](../../../extensibility/debugger/reference/ienumdebugaddresses-reset.md)|Setzt die Enumeration auf den ersten Eintrag zurück.|
|[Klonen](../../../extensibility/debugger/reference/ienumdebugaddresses-clone.md)|Ruft eine Kopie der aktuellen Enumeration ab.|
|[GetCount](../../../extensibility/debugger/reference/ienumdebugaddresses-getcount.md)|Ruft die Anzahl der Einträge in der-Enumeration ab.|

## <a name="remarks"></a>Bemerkungen
 Diese Schnittstelle wird in der Regel von der Debug-Engine verwendet, um die geeignete Adresse zu ermitteln, die der Ausdrucks Auswertung zugewiesen werden soll.

## <a name="requirements"></a>Anforderungen
 Header: sh. h

 Namespace: Microsoft. VisualStudio. Debugger. Interop

 Assembly: Microsoft.VisualStudio.Debugger.Interop.dll

## <a name="see-also"></a>Weitere Informationen
- [Symbol Provider Interfaces](../../../extensibility/debugger/reference/symbol-provider-interfaces.md)
- [IDebugAddress](../../../extensibility/debugger/reference/idebugaddress.md)
- [GetAddressesFromContext](../../../extensibility/debugger/reference/idebugsymbolprovider-getaddressesfromcontext.md)
- [GetAddressesFromPosition](../../../extensibility/debugger/reference/idebugsymbolprovider-getaddressesfromposition.md)
