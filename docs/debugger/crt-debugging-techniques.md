---
title: CRT-Debugverfahren | Microsoft-Dokumentation
ms.date: 11/04/2016
ms.topic: conceptual
f1_keywords:
- c.runtime.debugging
dev_langs:
- CSharp
- VB
- FSharp
- C++
helpviewer_keywords:
- debugging [CRT]
- CRT, debugging
- debugging [C++], CRT debug support
ms.assetid: 9be561f6-14a8-44ff-925d-d911d5b8e6ff
author: mikejo5000
ms.author: mikejo
manager: jillfra
ms.workload:
- multiple
ms.openlocfilehash: 88cdc78fd739de412b4cf796d0ca7a42f9174e0a
ms.sourcegitcommit: 94b3a052fb1229c7e7f8804b09c1d403385c7630
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "62564034"
---
# <a name="crt-debugging-techniques"></a>CRT-Debugverfahren
Die folgenden Debugverfahren können beim Debuggen von Programmen hilfreich sein, die die C-Laufzeitbibliothek verwenden.

## <a name="in-this-section"></a>In diesem Abschnitt
 [Verwenden der CRT-Debugbibliothek](../debugger/crt-debug-library-use.md)

 Hier wird beschrieben, wie die C-Laufzeitbibliothek das Debuggen unterstützt, und Sie erhalten Hinweise für den Zugriff auf die betreffenden Tools.

 [Makros für die Berichterstellung](../debugger/macros-for-reporting.md)

 Hier finden Sie Informationen zu den in CRTDBG.H definierten Makros **_RPTn** und **_RPTFn**, die anstelle von `printf`-Anweisungen zum Debuggen verwendet werden.

 [Debugversionen von Heapreservierungsfunktionen](../debugger/debug-versions-of-heap-allocation-functions.md)

 Erörtert die speziellen Debugversionen von Heapreservierungsfunktionen. Zu den behandelten Themen gehören die Zuordnung von Aufrufen durch die CRT-Laufzeitbibliothek, Vorteile des expliziten Aufrufs, Vermeiden von Konvertierungen, Dokumentieren der einzelnen Reservierungstypen in Clientblocks und die Ergebnisse bei nicht definiertem _DEBUG.

 [Details zum CRT-Debugheap](../debugger/crt-debug-heap-details.md)

 Enthält Links zu den Themen Speicherverwaltung und Debugheap, Blocktypen auf dem Debugheap, Verwenden des Debugheaps, Berichtsfunktionen für den Heapzustand und Nachverfolgen von Heapreservierungsanforderungen.

 [Schreiben von Hookfunktionen zum Debuggen](../debugger/debug-hook-function-writing.md)

 Enthält Links zu den Themen Hookfunktionen für Clientblöcke, Hookfunktionen für Reservierungen, Reservierungshooks und CRT-Speicherbelegungen sowie Hookfunktionen für Berichte.

 [Suchen von Arbeitsspeicherverlusten mit der CRT-Bibliothek](../debugger/finding-memory-leaks-using-the-crt-library.md)

 Hier werden Verfahren zum Erkennen und Isolieren von Arbeitsspeicherverlusten mithilfe des Debuggers und der C-Laufzeitbibliothek erläutert.

## <a name="related-sections"></a>Verwandte Abschnitte

- [Debuggen von nativem Code](../debugger/debugging-native-code.md): Hier werden einige allgemeine Probleme und Verfahren beim Debuggen für C- und C++-Anwendungen erörtert.
- [Debuggersicherheit](../debugger/debugger-security.md): Enthält Empfehlungen für mehr Sicherheit beim Debuggen.