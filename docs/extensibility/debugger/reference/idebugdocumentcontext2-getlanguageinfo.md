---
title: 'IDebugDocumentContext2:: getlanguageingefo | Microsoft-Dokumentation'
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugDocumentContext2::GetLanguageInfo
helpviewer_keywords:
- IDebugDocumentContext2::GetLanguageInfo
ms.assetid: 6a212ee5-414c-4eb5-ab11-19db1786943d
author: acangialosi
ms.author: anthc
manager: jillfra
ms.workload:
- vssdk
dev_langs:
- CPP
- CSharp
ms.openlocfilehash: 9d139029bf65149ae59fb037434f6e7d6298f1d5
ms.sourcegitcommit: 6cfffa72af599a9d667249caaaa411bb28ea69fd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2020
ms.locfileid: "80731858"
---
# <a name="idebugdocumentcontext2getlanguageinfo"></a>IDebugDocumentContext2::GetLanguageInfo
Ruft die Sprache ab, die diesem Dokument Kontext zugeordnet ist.

## <a name="syntax"></a>Syntax

```cpp
HRESULT GetLanguageInfo(
    BSTR* pbstrLanguage,
    GUID* pguidLanguage
);
```

```csharp
int GetLanguageInfo(
    out string pbstrLanguage,
    out Guid   pguidLanguage
);
```

## <a name="parameters"></a>Parameter
`pbstrLanguage`\
vorgenommen Gibt den Namen der Sprache zurück, die den Code in diesem Dokument Kontext implementiert.

`pguidLanguage`\
vorgenommen Gibt die GUID der Sprache zurück, die den Code in diesem Dokument Kontext implementiert.  Zum Beispiel: `guidVBScriptLang` oder `guidCPPLang`. Diese GUID ist nicht auf die von bereitgestellten Sprachen beschränkt [!INCLUDE[vsprvs](../../../code-quality/includes/vsprvs_md.md)] .

## <a name="return-value"></a>Rückgabewert
Wenn die Ausführung erfolgreich ist, wird `S_OK`, andernfalls ein Fehlercode zurückgegeben.

## <a name="example"></a>Beispiel
Im folgenden Beispiel wird gezeigt, wie diese Methode für ein einfaches-Objekt implementiert wird `CDebugContext` , das die [IDebugDocumentContext2](../../../extensibility/debugger/reference/idebugdocumentcontext2.md) -Schnittstelle verfügbar macht.

```cpp
HRESULT CDebugContext::GetLanguageInfo(BSTR* pbstrLanguage, GUID* pguidLanguage)
{
    HRESULT hr;

    // Check for a valid language argument pointers.
    if (pbstrLanguage && pguidLanguage)
    {
        *pguidLanguage = GUID_NULL;
        *pbstrLanguage = SysAllocString(L"Batch File");
        if (*pbstrLanguage)
        {
            *pguidLanguage = guidBatLang;
            hr = S_OK;
        }
        else
        {
            hr = E_OUTOFMEMORY;
        }
    }
    else
    {
        hr = E_INVALIDARG;
    }

    return hr;
}
```

## <a name="see-also"></a>Weitere Informationen
- [IDebugDocumentContext2](../../../extensibility/debugger/reference/idebugdocumentcontext2.md)
