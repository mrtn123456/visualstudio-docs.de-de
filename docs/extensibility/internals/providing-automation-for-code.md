---
title: Bereitstellen von Automatisierung für Code | Microsoft-Dokumentation
ms.date: 11/04/2016
ms.topic: conceptual
helpviewer_keywords:
- CodeModel object
ms.assetid: 21cb3e63-f25c-404b-bc1d-a32ad0fdd4d5
author: acangialosi
ms.author: anthc
manager: jillfra
ms.workload:
- vssdk
ms.openlocfilehash: bd13b7db2065069ff1540dbfc921570c2b230b8a
ms.sourcegitcommit: 6cfffa72af599a9d667249caaaa411bb28ea69fd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2020
ms.locfileid: "80705996"
---
# <a name="providing-automation-for-code"></a>Bereitstellen von Automatisierung für Code
Das Erstellen eines Automatisierungs Modells für Ihren Code ist nicht erforderlich. Das Umgebungs-SDK bietet hierfür kein Beispiel. Einen Einblick in Code Modelle finden Sie unter dem- <xref:EnvDTE.CodeModel> Objekt.

 Zum Implementieren eines Code Modells müssen Sie alle Schnittstellen implementieren, die von der internen Datenstruktur bestimmt werden. Die Objekte müssen von der-Klasse abgeleitet werden `IDispatch` .

 Die-Objekte, die Sie erweitern, <xref:EnvDTE.CodeModel> und <xref:EnvDTE.FileCodeModel> sind über das- <xref:EnvDTE.Project> Objekt verfügbar und sehen wie folgt aus:

- <xref:EnvDTE.Project.CodeModel%2A>

- <xref:EnvDTE.ProjectItem.FileCodeModel%2A>

 Sie können auswählen, dass Sie nur die `CodeModel` `FileCodeModel` -Schnittstelle oder die-Schnittstelle in dem-Objekt implementieren, das Sie von den `Project` <xref:EnvDTE.ProjectItem> Objekten und Stellen Sie eine beliebige Funktionalität von dieser Schnittstelle bereit, die für Ihr Projekt System geeignet ist.

 Wenn Sie Funktionen hinzufügen möchten, z. b. Methoden oder Eigenschaften, die nicht über die Standard `CodeModel` -und- `FileCodeModel` Schnittstellen verfügbar sind, erstellen Sie eine eigene Schnittstelle, die vom Standard erbt. Stellen Sie sicher, dass Sie Sie mit Ihrem Projekt System dokumentieren, damit Endbenutzer darauf achten können. Sie geben die Standardschnittstelle zurück, aber der Benutzer kann die-Methode oder eine Umwandlung in die-Schnittstelle durchsetzen, `QueryInterface` Wenn bekannt ist, dass Sie vorhanden ist.

## <a name="see-also"></a>Weitere Informationen
- [Übersicht über das Automatisierungsmodell](../../extensibility/internals/automation-model-overview.md)
