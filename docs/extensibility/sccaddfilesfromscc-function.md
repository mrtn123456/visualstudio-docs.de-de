---
title: Sccaddfilesfromscc-Funktion | Microsoft-Dokumentation
ms.date: 11/04/2016
ms.topic: conceptual
f1_keywords:
- SccAddFilesFromSCC
helpviewer_keywords:
- SccAddFilesFromSCC function
ms.assetid: f21a3500-ade8-4dd8-8647-10e2179be9c1
author: acangialosi
ms.author: anthc
manager: jillfra
ms.workload:
- vssdk
ms.openlocfilehash: 1d22527644edbf1697112f5cf8b73b8a3f72b774
ms.sourcegitcommit: 6cfffa72af599a9d667249caaaa411bb28ea69fd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2020
ms.locfileid: "80701291"
---
# <a name="sccaddfilesfromscc-function"></a>Sccaddfilesfromscc-Funktion
Diese Funktion fügt eine Liste von Dateien aus der Quell Code Verwaltung dem aktuell geöffneten Projekt hinzu.

## <a name="syntax"></a>Syntax

```cpp
SCCRTN SccAddFilesFromSCC(
   LPVOID  pContext,
   HWND    hWnd,
   LPSTR   lpUser,
   LPSTR   lpAuxProjPath,
   LONG    cFiles,
   LPCSTR* lpFilePaths,
   LPCSTR  lpDestination,
   LPCSTR  lpComment,
   LPBOOL  pbResults
);
```

### <a name="parameters"></a>Parameter
 pContext

in Der Kontext Zeiger für das Quellcodeverwaltungs-Plug-in.

 hWnd

in Ein Handle für das IDE-Fenster, das vom Quellcodeverwaltungs-Plug-in als übergeordnetes Element für alle bereitgestellten Dialogfelder verwendet werden kann.

 lpuser

[in, out] Der Benutzername (bis zu SCC_USER_SIZE, einschließlich des NULL-Terminator).

 lpauxprojpath

[in, out] Zusätzliche Zeichenfolge, die das Projekt identifiziert (bis zur `SCC_PRJPATH_` Größe, einschließlich des NULL-Terminator).

 cFiles

in Anzahl von Dateien, die von angegeben werden `lpFilePaths` .

 lpfilepath

[in, out] Array von Dateinamen, die dem aktuellen Projekt hinzugefügt werden sollen.

 lpdestination

in Der Zielpfad, in den die Dateien geschrieben werden sollen.

 lpcomment

in Der Kommentar, der auf jede der hinzugefügten Dateien angewendet werden soll.

 pbresults

[in, out] Ein Array von Flags, die festgelegt werden, um einen Erfolg (ungleich 0 oder true) oder einen Fehler (null oder false) für jede Datei anzugeben (die Größe des Arrays muss mindestens `cFiles` lang sein).

## <a name="return-value"></a>Rückgabewert
 Es wird erwartet, dass die Plug-in-Implementierung der Quell Code Verwaltung diese Funktion einen der folgenden Werte zurückgibt:

|Wert|BESCHREIBUNG|
|-----------|-----------------|
|SCC_E_PROJNOTOPEN|Das Projekt ist nicht geöffnet.|
|SCC_E_OPNOTPERFORMED|Die Verbindung ist nicht mit dem Projekt identisch, das von angegeben wird. `lpAuxProjPath.`|
|SCC_E_NOTAUTHORIZED|Der Benutzer ist nicht autorisiert, die Datenbank zu aktualisieren.|
|SCC_E_NONSPECIFICERROR|Unbekannter Fehler.|
|SCC_I_RELOADFILE|Eine Datei oder ein Projekt muss erneut geladen werden.|

## <a name="see-also"></a>Weitere Informationen
- [API-Funktionen der Quellcodeverwaltungs-Plug-in](../extensibility/source-control-plug-in-api-functions.md)
