---
title: Refactoring des Entfernens von nicht erreichbarem Code
ms.date: 03/10/2020
ms.topic: reference
author: mikadumont
ms.author: midumont
manager: jillfra
dev_langs:
- CSharp
- VB
ms.workload:
- dotnet
ms.openlocfilehash: cd827870f07fb3161674d287d20f266942e61afe
ms.sourcegitcommit: cc841df335d1d22d281871fe41e74238d2fc52a6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/18/2020
ms.locfileid: "79093961"
---
# <a name="remove-unreachable-code-refactoring"></a>Refactoring des Entfernens von nicht erreichbarem Code

Dieses Refactoring gilt für:

- C#

- Visual Basic

**Beschreibung**: Es wird Code entfernt, der nie ausgeführt wird.

**Hintergrund**: Ihr Programm enthält keinen Pfad zu einem bestimmten Codeausschnitt, weshalb dieser Codeausschnitt nicht benötigt wird.

**Vorteile**: Die Lesbarkeit und Verwaltbarkeit werden durch das Entfernen eines überflüssigen, nie ausgeführten Code verbessert.

## <a name="how-to"></a>Vorgehensweise

1. Platzieren Sie den Cursor an eine beliebige Stelle im ausgeblendeten, nicht erreichbaren Code:

![Ausgeblendeter nicht erreichbarer Code](media/unreachablecode-faded-cs.png)

1. Führen Sie dann eine der folgenden Aktionen aus:

   - **Tastatur**
      - Drücken Sie an einer beliebigen Stelle in einer Zeile **STRG**+ **.** , um das Menü **Schnellaktionen und Refactorings** aufzurufen, und wählen Sie im Popupvorschaufenster **Nicht erreichbaren Code entfernen** aus.
   - **Maus**
      - Klicken Sie mit der rechten Maustaste auf den Code, und wählen Sie das Menü **Schnellaktionen und Refactorings** sowie im Popupvorschaufenster **Nicht erreichbaren Code entfernen** aus.

1. Wenn Sie mit der Änderung zufrieden sind, drücken Sie die **EINGABETASTE**, oder klicken Sie im Menü auf die Korrektur. Die Änderungen werden angewendet.

Beispiel:

```csharp
// Before
private void Method()
{
    throw new Exception(nameof(Method));
    Console.WriteLine($"Exception for method {nameof(Method)}");
}

// Remove unreachable code

// After
private void Method()
{
    throw new Exception(nameof(Method));
}
```

## <a name="see-also"></a>Weitere Informationen

- [Refactoring](../refactoring-in-visual-studio.md)
- [Vorschau der Änderungen](../../ide/preview-changes.md)
