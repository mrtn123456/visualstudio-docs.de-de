---
title: Befehl Verträge im Interop-Assemblys | Microsoft-Dokumentation
ms.custom: ''
ms.date: 2018-06-30
ms.prod: visual-studio-dev14
ms.reviewer: ''
ms.suite: ''
ms.technology:
- vs-ide-sdk
ms.tgt_pltfrm: ''
ms.topic: article
helpviewer_keywords:
- command handling with interop assemblies, command contracts
- interop assemblies, command contracts
ms.assetid: 57245708-f539-42dc-8963-2754a48f0189
caps.latest.revision: 14
ms.author: gregvanl
manager: ghogen
ms.openlocfilehash: 8a5e2a7abb298aa43aefbf3f04c048c5928bd555
ms.sourcegitcommit: 55f7ce2d5d2e458e35c45787f1935b237ee5c9f8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2018
ms.locfileid: "47511587"
---
# <a name="command-contracts-in-interop-assemblies"></a>Befehlsverträge in Interop-Assemblys
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

Die neueste Version dieses Themas finden Sie unter [Befehlsverträge in Interop-Assemblys](https://docs.microsoft.com/visualstudio/extensibility/internals/command-contracts-in-interop-assemblies).  
  
Der Basisvertrag für die Behandlung von Befehlen über die <xref:Microsoft.VisualStudio.OLE.Interop.IOleCommandTarget> Schnittstelle ist, dass die Umgebung Ruft die <xref:Microsoft.VisualStudio.OLE.Interop.IOleCommandTarget.QueryStatus%2A> Methode, um zu bestimmen, ob der Befehl unterstützt wird, und es unterstützt wird, um dessen Zustand und den Text zu bestimmen. Anschließend ruft die Umgebung die <xref:Microsoft.VisualStudio.OLE.Interop.IOleCommandTarget.Exec%2A> Methode zum Ausführen des Befehls.  
  
 Die <xref:Microsoft.VisualStudio.OLE.Interop.IOleCommandTarget.QueryStatus%2A> Methode erfolgt genauso wie für alle Befehle. Weitere Kommunikation, bei Bedarf (z. B. mit Dropdownlisten), wird durch den Aufruf verwaltet die <xref:Microsoft.VisualStudio.OLE.Interop.IOleCommandTarget.Exec%2A> Methode mit entsprechenden Parametern. Die Interpretation dieser Parameter hängt von den angegebenen Befehl ab.  
  
 Wenn das Ziel des Befehls die Werte in der Output-Parameter zurückgibt, ist der Aufrufer immer verantwortlich für das Freigeben von Ressourcen, die zugeordnet war. Da dieser Parameter auf einen Variant-Wert ist, gibt die Variante Löschen der Ressourcen frei.  
  
 In Fällen, in denen Befehle ausgeführt in einem Fenster "Aufrufhierarchie werden müssen" die <xref:Microsoft.VisualStudio.Shell.Interop.IVsUIHierarchy> Schnittstelle muss verwendet werden. Die <xref:Microsoft.VisualStudio.Shell.Interop.IVsUIHierarchy> Schnittstelle verfügt über ein ähnlicher Vertrag mit ähnlichen Methoden: <xref:Microsoft.VisualStudio.Shell.Interop.IVsUIHierarchy.QueryStatusCommand%2A> und <xref:Microsoft.VisualStudio.Shell.Interop.IVsUIHierarchy.ExecCommand%2A>.  
  
## <a name="see-also"></a>Siehe auch  
 [Wie VSPackages Benutzeroberflächenelemente hinzufügen](../../extensibility/internals/how-vspackages-add-user-interface-elements.md)   
 [Befehlsrouting in VSPackages](../../extensibility/internals/command-routing-in-vspackages.md)   
 [Implementation (Implementierung)](../../extensibility/internals/command-implementation.md)
