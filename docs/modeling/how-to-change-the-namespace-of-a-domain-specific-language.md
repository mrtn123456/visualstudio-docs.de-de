---
title: 'Vorgehensweise: Ändern des Namespace einer domänenspezifischen Sprache'
description: Enthält Informationen zum Ändern des Namespace einer domänenspezifischen Sprache.
ms.date: 10/31/2018
ms.topic: how-to
titleSuffix: ''
helpviewer_keywords:
- Domain-Specific Language, namespace
author: JoshuaPartlow
ms.author: joshuapa
manager: jillfra
ms.custom: SEO-VS-2020
ms.workload:
- multiple
ms.openlocfilehash: a7b0de26fdc1a7982347a12c283a6aa73e9aad12
ms.sourcegitcommit: 566144d59c376474c09bbb55164c01d70f4b621c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/19/2020
ms.locfileid: "90809439"
---
# <a name="how-to-change-the-namespace-of-a-domain-specific-language"></a>Vorgehensweise: Ändern des Namespace einer domänenspezifischen Sprache

Sie können den Namespace einer domänenspezifischen Sprache ändern. Nehmen Sie die Änderung im **DSL-Explorer**, in den Eigenschaften des DSL-Paket Projekts und in den Assemblyinformationen vor.

## <a name="to-change-the-namespace-of-a-domain-specific-language"></a>So ändern Sie den Namespace einer domänenspezifischen Sprache

1. Wählen Sie im **DSL-Explorer**den Knoten **DSL** aus.

2. Ändern Sie im **Eigenschaften** Fenster die Eigenschaft **Namespace** .

3. Speichern Sie die Projekt Mappe, und transformieren Sie die Vorlagen.

4. Wählen Sie im Menü **Projekt** die Option **DSL-Eigenschaften**aus.

   Die Eigenschaften für das Projekt werden angezeigt.

5. Wählen Sie die Registerkarte **Anwendung** aus.

6. Ändern Sie die Eigenschaft **Standard Namespace** in den neuen Namespace Namen.

7. Wenn Sie auch den Namen der Assembly ändern möchten, ändern Sie die **Eigenschaft AssemblyName.**

8. Wenn Sie den Assemblynamen geändert haben, öffnen Sie dslpackage\package.tt, und aktualisieren Sie diese Zeile:

   `string dslAssembly = "YourDSLassembly.Dsl.dll";`

9. Wenn Sie benutzerdefinierten Code geschrieben haben, stellen Sie sicher, dass Sie den Namespace und die Klassen Verweise in den Code Dateien ändern.

10. Setzen Sie die experimentelle Instanz von Visual Studio zurück.

    1. Löschen Sie **\Users \\ **_{Your Name}_**\appdata\local\microsoft\visualstudio \\ \* Exp**.

    2. Wählen Sie im Windows- **Startmenü** **Alle Programme**aus,  >  **Microsoft Visual Studio**  >  **Tools**  >  **die experimentelle Instanz**2010 SDK-Tools zurücksetzen.

11. Wählen Sie im Menü **Erstellen** die Option Projekt Mappe **neu erstellen**aus.

## <a name="see-also"></a>Siehe auch

[Glossar für domänenspezifische Sprach Tools](/previous-versions/bb126564(v=vs.100))