---
title: Verwendung der CRT-Debugbibliothek | Microsoft-Dokumentation
ms.date: 10/03/2019
ms.topic: conceptual
f1_keywords:
- c.debug.runtime
dev_langs:
- CSharp
- VB
- FSharp
- C++
helpviewer_keywords:
- /DEBUG linker option [C++]
- crtdbg.h file
- debug library
- MDd compiler option [C++]
- libraries, CRT debug library
- MTd compiler option [C++]
- LDd compiler function [C++]
- /MTd compiler option [C++]
- /MDd compiler option [C++]
- debugging [CRT], CRT debug library
- DEBUG linker option [C++]
- /LDd compiler function [C++]
ms.assetid: 464de16b-4215-4787-9bfa-921aaff9d9f4
author: mikejo5000
ms.author: mikejo
manager: jillfra
ms.workload:
- multiple
ms.openlocfilehash: 20aeee220bec600c2232286d18600b04201ad03b
ms.sourcegitcommit: 5f6ad1cefbcd3d531ce587ad30e684684f4c4d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/22/2019
ms.locfileid: "72745609"
---
# <a name="crt-debug-library-use"></a>Verwenden der CRT-Debugbibliothek
Die C-Laufzeitbibliothek bietet umfassende Debugunterstützung. Um eine der CRT-Debugbibliotheken verwenden zu können, müssen eine Verknüpfung mit [/DEBUG](/cpp/build/reference/debug-generate-debug-info) und eine Kompilierung mit **/MDd**, **/MTd** oder **/LDd** durchgeführt werden.

## <a name="remarks"></a>Hinweise
 Die Hauptdefinitionen und Makros für CRT-Debugverfahren befinden sich in der Headerdatei Crtdbg.h.

 Die Funktionen in den CRT-Debugbibliotheken werden mit Debuginformationen ([/Z7, /Zd, /Zi, /ZI (Debuginformationsformat)](/cpp/build/reference/z7-zi-zi-debug-information-format)) und ohne Optimierung kompiliert. Einige der Funktionen enthalten Assertionen, um die an sie übergebenen Parameter zu überprüfen. Außerdem ist Quellcode enthalten. Mit diesem Quellcode können Sie in die CRT-Funktionen springen, um sicherzustellen, dass sie erwartungsgemäß funktionieren, und fehlerhafte Parameter oder Speicherzustände suchen. (Einige CRT-Laufzeittechnologien sind jedoch proprietär und beinhalten daher keinen Quellcode für Ausnahmebehandlung, Gleitkomma- und einige andere Routinen.)

 Weitere Informationen zum Verwenden der verschiedenen Laufzeitbibliotheken finden Sie unter [C-Laufzeitbibliotheken](/cpp/c-runtime-library/crt-library-features).

## <a name="see-also"></a>Siehe auch

- [CRT-Debugverfahren](../debugger/crt-debugging-techniques.md)
- [/MD, /MT, /LD (Laufzeitbibliothek verwenden)](/cpp/build/reference/md-mt-ld-use-run-time-library)