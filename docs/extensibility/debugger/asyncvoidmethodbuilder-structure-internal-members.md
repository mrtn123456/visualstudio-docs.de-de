---
title: 'Asyncvoidmethodbuilder-Struktur: interne Member | Microsoft-Dokumentation'
ms.date: 11/04/2016
ms.topic: conceptual
helpviewer_keywords:
- debug engines, AsyncVoidMethodBuilder structure [.NET Framework]
- AsyncVoidMethodBuilder structure [.NET Framework debug engines]
ms.assetid: fe2970ab-d4c5-4355-a8e4-772ee0a57178
author: acangialosi
ms.author: anthc
manager: jillfra
ms.workload:
- vssdk
ms.openlocfilehash: 866a53fae7bb2cc5325112b84d992da6f95af246
ms.sourcegitcommit: 6cfffa72af599a9d667249caaaa411bb28ea69fd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2020
ms.locfileid: "80739303"
---
# <a name="asyncvoidmethodbuilder-structure---internal-members"></a>Asyncvoidmethodbuilder-Struktur: interne Member
In diesem Thema werden die internen Member der- <xref:System.Runtime.CompilerServices.AsyncVoidMethodBuilder> Klasse beschrieben. Allgemeine Informationen zu dieser Klasse finden Sie im <xref:System.Runtime.CompilerServices.AsyncVoidMethodBuilder> Referenz Thema.

 **Namespace:** <xref:System.Runtime.CompilerServices?displayProperty=fullName>

 **Assembly:** mscorlib (in mscorlib.dll)

 Da Sie nicht auf diese internen Member vom .NET Framework aus zugreifen können, wird die folgende Syntax in Common Intermediate Language (CIL) bereitgestellt.

## <a name="syntax"></a>Syntax

```csharp
.class public sequential ansi sealed beforefieldinit System.Runtime.CompilerServices.AsyncVoidMethodBuilder
       extends System.ValueType
       implements System.Runtime.CompilerServices.IAsyncMethodBuilder
```

## <a name="internal-members"></a>Interne Member

|Name|BESCHREIBUNG|
|----------|-----------------|
|[Objectidfordebugger-Eigenschaft](../../extensibility/debugger/asyncvoidmethodbuilder-objectidfordebugger-property.md)|Ruft ein Objekt ab, das verwendet werden kann, um diesen Generator für den Debugger eindeutig zu identifizieren.|
|[m_objectIdForDebugger Feld](../../extensibility/debugger/asyncvoidmethodbuilder-m-objectidfordebugger-field.md)|Stellt das verzögert initialisierte Objekt dar, das vom Debugger verwendet wird, um diesen Generator eindeutig zu identifizieren.|

## <a name="see-also"></a>Weitere Informationen
- <xref:System.Runtime.CompilerServices.AsyncVoidMethodBuilder>
- [Parallele Erweiterungs internale für die .NET Framework](../../extensibility/debugger/parallel-extension-internals-for-the-dotnet-framework.md)
