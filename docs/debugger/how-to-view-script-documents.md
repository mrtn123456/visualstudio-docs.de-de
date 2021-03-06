---
title: Anzeigen von Skriptdokumenten | Microsoft-Dokumentation
ms.date: 11/05/2019
ms.topic: how-to
dev_langs:
- CSharp
- VB
- FSharp
- C++
helpviewer_keywords:
- Script Explorer
ms.assetid: 8b621e53-4508-4b4a-9995-70995b0b9ac8
author: mikejo5000
ms.author: mikejo
manager: jillfra
ms.workload:
- multiple
ms.openlocfilehash: 5f6d60d11737cde2beebdaeeccae8e547df78853
ms.sourcegitcommit: 062615c058d2ff44751e8d0c704ccfa3c5543469
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2020
ms.locfileid: "90851033"
---
# <a name="how-to-view-script-documents-javascript"></a>Vorgehensweise: Anzeigen von Dokumenten (JavaScript)

Serverseitige Skriptdateien sind im Projektmappen-Explorer sichtbar. Clientseitige Skriptdateien sind nur sichtbar, wenn Sie sich im Debugmodus oder Unterbrechungsmodus befinden. Clientseitige Skriptdateien werden im Knoten **Skriptdokumente** angezeigt.

Für einige Anwendungstypen, die Seiten dynamisch generieren, ist es einfacher, in den Unterbrechungsmodus überzugehen und zu debuggen, wenn Sie einen Haltepunkt aus einem Skriptdokument festlegen, das im Browser geladen wird. Entsprechend können Sie die `debugger`-Anweisung aus einem geladenen Skriptdokument hinzufügen, um in den Unterbrechungsmodus zu wechseln. In diesem Artikel wird gezeigt, wie Sie diese Dokumente anzeigen.

> [!NOTE]
> Vor Version [!INCLUDE[vs_dev11_long](../data-tools/includes/vs_dev11_long_md.md)] wurden clientseitige Skriptdateien, die durch Skripts auf Serverseite generiert wurden, im Fenster Skript-Explorer angezeigt.

### <a name="to-view-a-server-side-script-document"></a>So zeigen Sie ein serverseitiges Skriptdokument an

1. Öffnen Sie im **Projektmappen-Explorer** den Knoten **\<Website Pathname>** .

2. Doppelklicken Sie auf die Skriptdatei, die Sie anzeigen möchten.

     Die serverseitige Skriptdatei wird in einem Quellcodefenster geöffnet.

### <a name="to-view-a-client-side-script-document"></a>So zeigen Sie ein clientseitiges Skriptdokument an

1. Öffnen Sie im **Projektmappen-Explorer** den Knoten **Skriptdokumente**.

2. Doppelklicken Sie auf die Skriptdatei, die Sie anzeigen möchten.

     Die clientseitige Skriptdatei wird in einem Quellcodefenster geöffnet.

## <a name="see-also"></a>Siehe auch
- [Anzeigen von Daten im Debugger](../debugger/viewing-data-in-the-debugger.md)