---
title: Neuerungen bei der Profilerstellung in Visual Studio 2017 | Microsoft-Dokumentation
titleSuffix: ''
ms.date: 11/04/2016
ms.topic: conceptual
helpviewer_keywords:
- profiling
- what's new
ms.assetid: d4736cc8-8961-4089-be9e-d5190ce8353c
author: mikejo5000
ms.author: mikejo
manager: jillfra
ms.workload:
- multiple
monikerRange: vs-2017
ms.openlocfilehash: 0512c6e95f0a26184593f7af5ba08c31c33a3299
ms.sourcegitcommit: cc841df335d1d22d281871fe41e74238d2fc52a6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/18/2020
ms.locfileid: "71128341"
---
# <a name="whats-new-in-profiling-tools-in-includevs_dev15"></a>Neuerungen bei den Profilerstellungstools in [!include[vs_dev15](../misc/includes/vs_dev15_md.md)]

Die Diagnosetools enthalten neue Visualisierungen, um Ihnen bei der Identifizierung von Problemen in Ihrer App zu helfen, die behoben werden müssen. Die Diagnosetools umfassen jetzt Unterstützung für ASP.NET-Apps.

Weitere Informationen finden Sie in den [Anmerkungen zu [!include[vs_dev15](../misc/includes/vs_dev15_md.md)]](/visualstudio/releasenotes/vs2017-relnotes).

Zu den Tools wurde eine Registerkarte **Zusammenfassung** hinzugefügt, die Ihnen dabei hilft, den Fokus für Ihre Leistungsanalyse auf die Hauptbereiche zu legen. Diese Registerkarte zeigt, wie viele Ereignisse aufgetreten sind, lässt Sie Momentaufnahmen des Heaps machen und schnell die Datensammlung für die CPU-Auslastung aktivieren. In dieser Ansicht werden alle Ereignisse von [Application Insights](/azure/azure-monitor/app/visual-studio) oder der [Analyse der Benutzeroberfläche](/visualstudio/releasenotes/vs2017-relnotes) gezeigt. Darüber hinaus werden in dieser Ansicht auch IntelliTrace-Ereignisse für Visual Studio Enterprise gezeigt.

![Registerkarte „Zusammenfassung“ der Diagnosetools](../profiling/media/diag-tools-summary-tab-2.png "DiagToolsSummaryTab")

Das Tool für die CPU-Auslastung verfügt über [neue Visualisierungen](../profiling/Beginners-Guide-to-Performance-Profiling.md), um Ihnen beim Identifizieren der Funktionen zu helfen, die am wahrscheinlichsten Leistungsprobleme verursachen. Die neue Ansicht **Aufrufer/Aufgerufener** können Sie zum Untersuchen der Kosten von Funktionsaufrufen verwenden, die an eine und von einer ausgewählten Funktion erfolgen.

![Ansicht „Aufrufer/Aufgerufener“ der Diagnosetools](../profiling/media/diag-tools-caller-callee-2.png "DiagToolsCallerCallee")

## <a name="see-also"></a>Siehe auch

- [Profilerstellung in Visual Studio](../profiling/index.yml)
- [Einführung in Profilerstellungstools](../profiling/profiling-feature-tour.md)