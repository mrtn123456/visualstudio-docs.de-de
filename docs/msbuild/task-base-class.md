---
title: Task-Basisklasse | Microsoft-Dokumentation
description: Erfahren Sie mehr über die Parameter, die die Basisklasse „Microsoft.Build.Utilities.Task“ den Aufgaben hinzufügt, die von ihr erben.
ms.custom: SEO-VS-2020
ms.date: 11/04/2016
ms.topic: reference
dev_langs:
- VB
- CSharp
- C++
- jsharp
ms.assetid: 6c3f6238-b9f0-4325-b8b0-de61090bd0a2
author: ghogen
ms.author: ghogen
manager: jillfra
ms.workload:
- multiple
ms.openlocfilehash: 41557eb7df3da8a6322a3951520918ffb158b57a
ms.sourcegitcommit: 1a36533f385e50c05f661f440380fda6386ed3c1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/30/2020
ms.locfileid: "93048000"
---
# <a name="task-base-class"></a>Aufgabenbasisklasse

Viele Aufgaben erben letztlich von der <xref:Microsoft.Build.Utilities.Task>-Klasse. Diese Klasse fügt den Aufgaben, die ihr abgeleitet werden, mehrere Parameter hinzu. Diese Parameter werden in diesem Dokument aufgeführt.

## <a name="parameters"></a>Parameter

 In der folgenden Tabelle werden die Parameter dieser Basisklasse beschrieben.

|Parameter|Beschreibung|
|---------------|-----------------|
|<xref:Microsoft.Build.Utilities.Task.BuildEngine%2A>|Optionaler <xref:Microsoft.Build.Framework.IBuildEngine>-Parameter.<br /><br /> Gibt die für die Aufgaben verfügbare Build-Engine-Schnittstelle an. Die Build-Engine legt diesen Parameter automatisch fest, damit Aufgaben zurückgerufen werden können.|
|<xref:Microsoft.Build.Utilities.Task.BuildEngine2%2A>|Optionaler <xref:Microsoft.Build.Framework.IBuildEngine2>-Parameter.<br /><br /> Gibt die für die Aufgaben verfügbare Build-Engine-Schnittstelle an. Die Build-Engine legt diesen Parameter automatisch fest, damit Aufgaben zurückgerufen werden können.<br /><br /> Hierbei handelt es sich um eine benutzerfreundliche Eigenschaft. Daher müssen die von dieser Klasse erbenden Aufgabenautoren den Wert nicht von `IBuildEngine` zu `IBuildEngine2` umwandeln.|
|<xref:Microsoft.Build.Utilities.Task.BuildEngine3%2A>|Optionaler <xref:Microsoft.Build.Framework.IBuildEngine3>-Parameter.<br /><br /> Gibt die durch den Host bereitgestellte Build-Engine-Schnittstelle an.|
|<xref:Microsoft.Build.Utilities.Task.HostObject%2A>|Optionaler <xref:Microsoft.Build.Framework.ITaskHost>-Parameter.<br /><br /> Gibt die Hostobjektinstanz (kann null sein) an. Die Build-Engine legt diese Eigenschaft fest, wenn die Host-IDE ein Hostobjekt mit dieser bestimmten Aufgabe verknüpft hat.|
|<xref:Microsoft.Build.Utilities.Task.Log%2A>|Optionaler schreibgeschützter <xref:Microsoft.Build.Utilities.TaskLoggingHelper>-Parameter.<br /><br /> Das Hilfsobjekt für die Protokollierung|

## <a name="see-also"></a>Weitere Informationen

- [Referenz zu MSBuild-Tasks](../msbuild/msbuild-task-reference.md)
- [Aufgaben](../msbuild/msbuild-tasks.md)
