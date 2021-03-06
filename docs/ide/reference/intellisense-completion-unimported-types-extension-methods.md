---
title: IntelliSense-Vervollständigung für Typen und Erweiterungsmethoden
description: In diesem Artikel erfahren Sie, wie Sie die IntelliSense-Vervollständigung und Erweiterungsmethoden verwenden, die Sie noch nicht mithilfe einer `using`-Anweisung importiert haben.
ms.custom: SEO-VS-2020
ms.date: 07/27/2020
ms.topic: reference
author: mikadumont
ms.author: midumont
manager: jillfra
dev_langs:
- CSharp
- VB
ms.workload:
- dotnet
ms.openlocfilehash: d2ac806b4a83b23a783c59eeee5df801c9237685
ms.sourcegitcommit: 86e98df462b574ade66392f8760da638fe455aa0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/19/2020
ms.locfileid: "94900919"
---
# <a name="intellisense-completion-for-unimported-types-and-extension-methods"></a>IntelliSense-Vervollständigung für nicht importierte Typen und Erweiterungsmethoden

Dieses Refactoring gilt für:

- C#

- Visual Basic

**Beschreibung:** IntelliSense stellt die Vervollständigung für nicht importierte Typen und Erweiterungsmethoden bereit.

**Hintergrund:** Wenn Sie einen Typ oder Erweiterungsmethoden verwenden möchten, für die in Ihrem Projekt bereits eine Abhängigkeit vorhanden ist, aber die using-Anweisung wurde noch nicht zu Ihrer Datei hinzugefügt.

**Vorteile**: Somit müssen Sie die using-Anweisung nicht manuell zu Ihrer Datei hinzufügen.

## <a name="how-to"></a>Vorgehensweise

1. Sobald Sie damit beginnen, den Namen eines Typs oder einer Erweiterungsmethode einzugeben, für die eine Abhängigkeit in Ihrem Projekt vorhanden ist, stellt IntelliSense Vorschläge bereit. Für Elemente aus nicht importierten Namespaces wird der enthaltende Namespace als Suffix angezeigt.

   > [!TIP]
   > Sie können Elemente mithilfe der **Expander-Schaltfläche (ALT+A)** aus nicht importierten Namespaces nach Bedarf anzeigen und ausblenden, die unten links von der Vervollständigungsliste angezeigt wird. Zum Ändern des Standardverhaltens navigieren Sie zu **Extras** > **Optionen** > **Text-Editor** > **C#**  / **Allgemein** > **IntelliSense**, und suchen Sie dort nach der Option **Elemente aus nicht importierten Namespaces anzeigen**.

2. Wählen Sie ein nicht importiertes Element aus, und committen Sie dieses.

   Die using-Anweisung wird automatisch zu Ihrer Datei hinzugefügt.

   ![IntelliSense-Vervollständigung für nicht importierte Typen](media/intellisense-completion-unimported-types.png)

## <a name="see-also"></a>Siehe auch

- [IntelliSense](../using-intellisense.md)
- [Refactoring](../refactoring-in-visual-studio.md)
