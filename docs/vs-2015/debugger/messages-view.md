---
title: Meldungsansicht | Microsoft-Dokumentation
ms.custom: ''
ms.date: 2018-06-30
ms.prod: visual-studio-dev14
ms.reviewer: ''
ms.suite: ''
ms.technology:
- vs-ide-debug
ms.tgt_pltfrm: ''
ms.topic: article
f1_keywords:
- vs.externaltools.spyplus.messagesview
helpviewer_keywords:
- Messages view
ms.assetid: 14c2a786-c23a-4b2d-acad-8c32a856c70d
caps.latest.revision: 9
author: mikejo5000
ms.author: mikejo
manager: ghogen
ms.openlocfilehash: 7d603ad157786df756f130c3bf203961b48a610f
ms.sourcegitcommit: 55f7ce2d5d2e458e35c45787f1935b237ee5c9f8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2018
ms.locfileid: "47522724"
---
# <a name="messages-view"></a>Meldungsansicht
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

Die neueste Version dieses Themas finden Sie unter [Meldungsansicht](https://docs.microsoft.com/visualstudio/debugger/messages-view).  
  
Jedes Fenster verfügt über einen Stream zugeordnete Meldung. Ansichtsfenster Nachrichten wird Meldungsstream. Das Fensterhandle, Message Authentication Code und Meldung werden angezeigt. Sie können eine Ansicht "Nachrichten" für einen Thread oder Prozess sowie erstellen. Dadurch können Sie zum Anzeigen von Nachrichten an alle Fenster, die im Besitz von einem bestimmten Prozess oder Thread, der besonders nützlich für das Erfassen von fenstermeldungen für die Initialisierung ist.  
  
 Eine typische Ansicht Meldungsfenster wird unten angezeigt. Beachten Sie, dass die erste Spalte das Fensterhandle enthält, und die zweite Spalte einen Message Authentication Code enthält (beschrieben [Meldungscodes](../debugger/message-codes.md)). Decodierte Nachrichtenparameter und Rückgabewerte werden auf der rechten Seite.  
  
 ![Spy++&#43; &#43; Meldungsansicht](../debugger/media/spy-messagesview.png "Spy-_MessagesView")  
Spy++-Meldungsansicht  
  
## <a name="procedures"></a>Verfahren  
  
#### <a name="to-open-a-messages-view-for-a-window-process-or-thread"></a>Um eine Ansicht "Nachrichten" für ein Fenster, Prozess oder Thread zu öffnen.  
  
1.  Verschieben des Fokus um eine [Windows-Ansicht](../debugger/windows-view.md), [Prozessansicht](../debugger/processes-view.md), oder [Ansicht "Threads"](../debugger/threads-view.md) Fenster.  
  
2.  Suchen Sie den Knoten für das Element, dessen Nachrichten, die Sie untersuchen möchten, und wählen Sie ihn.  
  
3.  Von der **Spy** Menü wählen **Protokollmeldungen**.  
  
     Die [im Dialogfeld "Optionen" Nachricht](../debugger/message-options-dialog-box.md) wird geöffnet.  
  
4.  Wählen Sie die Optionen für die Nachricht, die Sie anzeigen möchten.  
  
5.  Drücken Sie **OK** zum Protokollieren von Nachrichten beginnen.  
  
     Ein Nachrichten, die Fenster "Berichtsansicht" geöffnet wird, sowie einen **Nachrichten** Menü zur Spy++-Symbolleiste hinzugefügt wird. Abhängig von den ausgewählten Optionen, Nachrichten mit dem streamen beginnen in das aktive Fenster des Nachrichten-Ansicht.  
  
6.  Wenn Sie über genügend Nachrichten verfügen, wählen Sie **Protokollierung beenden** aus der **Nachrichten** Menü.  
  
## <a name="in-this-section"></a>In diesem Abschnitt  
 [Steuern der Meldungsansicht](../debugger/how-to-control-messages-view.md)  
 Erläutert, wie zum Verwalten der Ansicht "Nachrichten".  
  
 [Suchen nach einer Nachricht in der Meldungsansicht](../debugger/how-to-search-for-a-message-in-messages-view.md)  
 Erläutert, wie Sie eine bestimmte Nachricht in der Ansicht "Nachrichten".  
  
 [Starten und Beenden der Meldungsprotokollanzeige](../debugger/how-to-start-and-stop-the-message-log-display.md)  
 Erläutert das Starten und beenden die nachrichtenprotokollierung.  
  
 [Meldungscodes](../debugger/message-codes.md)  
 Definiert die Codes für Nachrichten, die in der Ansicht "Nachrichten" aufgeführt.  
  
 [Anzeigen von Meldungseigenschaften](../debugger/how-to-display-message-properties.md)  
 So zeigen Sie weitere Informationen zu einer Meldung.  
  
## <a name="related-sections"></a>Verwandte Abschnitte  
 [Spy++-Ansichten](../debugger/spy-increment-views.md)  
 Erläutert die Spy++-Strukturansichten von Windows, Nachrichten, Prozesse und Threads.  
  
 [Verwenden von Spy++](../debugger/using-spy-increment.md)  
 Führt das Tool Spy++ und erläutert, wie sie verwendet werden kann.  
  
 [Dialogfeld "Meldungsoptionen"](../debugger/message-options-dialog-box.md)  
 Wird verwendet, um auszuwählen, welche Nachrichten in der aktiven Ansicht "Nachrichten" aufgeführt sind.  
  
 [Meldungssuche (Dialogfeld)](../debugger/message-search-dialog-box.md)  
 Verwendet, um den Knoten für eine bestimmte Nachricht in der Ansicht "Nachrichten" suchen.  
  
 [Dialogfeld "Meldungseigenschaften"](../debugger/message-properties-dialog-box.md)  
 Zum Anzeigen der Eigenschaften einer Nachricht, die ausgewählten Meldung verwendet.  
  
 [Spy++-Referenz](../debugger/spy-increment-reference.md)  
 Enthält Abschnitte, die jedes Spy++ Menü- und Dialogfeldressourcen Feld beschreibt.


