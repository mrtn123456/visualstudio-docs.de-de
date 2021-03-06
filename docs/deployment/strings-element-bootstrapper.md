---
title: '&lt;Strings- &gt; Element (Boots Trapper) | Microsoft-Dokumentation'
description: Das Strings-Element definiert lokalisierte Zeichen folgen für Produktnamen, Paketnamen und Installations Fehlermeldungen.
ms.custom: SEO-VS-2020
ms.date: 11/04/2016
ms.topic: conceptual
f1_keywords:
- MSBuild.GenerateBootstrapper.NoStringsForCulture
- MSBuild.GenerateBootstrapper.ProductCultureNotFound
dev_langs:
- FSharp
- VB
- CSharp
- C++
helpviewer_keywords:
- <Strings> element [bootstrapper]
ms.assetid: d5ea3613-5fc9-4a11-bef3-46a01178bf60
author: mikejo5000
ms.author: mikejo
manager: jillfra
ms.workload:
- multiple
ms.openlocfilehash: 09608f4b182d72b0b86b69df7df0b37d019ddf45
ms.sourcegitcommit: 75bfdaab9a8b23a097c1e8538ed1cde404305974
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/07/2020
ms.locfileid: "94350477"
---
# <a name="ltstringsgt-element-bootstrapper"></a>&lt;Strings- &gt; Element (Boots Trapper)
Definiert lokalisierte Zeichen folgen für Produktnamen, Paketnamen und Installations Fehlermeldungen.

## <a name="syntax"></a>Syntax

```xml
<Strings>
    <String
        Name
    >
    </String>
</Strings>
```

## <a name="elements-and-attributes"></a>Elemente und Attribute
 Das- `Strings` Element ist ein untergeordnetes `Package` Element des-Elements. Sie besitzt keine Attribute.

## <a name="string"></a>String
 Das- `String` Element ist ein untergeordnetes `Strings` Element des-Elements. Ein- `Strings` Element kann ein oder mehrere- `String` Elemente aufweisen.

 `String` weist das folgende Attribut auf.

|attribute|BESCHREIBUNG|
|---------------|-----------------|
|`Name`|Erforderlich. Der Name der Zeichenfolge.|

## <a name="example"></a>Beispiel
 Im folgenden Codebeispiel werden alle englischen Zeichen folgen für den .NET Framework Installer angegeben.

```xml
<Strings>
    <String Name="DisplayName">.NET Framework 2.0</String>
    <String Name="Culture">en</String>
    <String Name="AdminRequired">Administrator permissions are required to install the .NET Framework 2.0. Contact your administrator.</String>
    <String Name="InvalidPlatformWin9x">Installation of the .NET Framework 2.0 is not supported on Windows 95. Contact your application vendor.</String>
    <String Name="InvalidPlatformWinNT">Installation of the .NET Framework 2.0 is not supported on Windows NT 4.0. Contact your application vendor.</String>
    <String Name="InvalidPlatformIE">Installation of the .NET Framework 2.0 requires Internet Explorer 5.01 or greater. Contact your application vendor.</String>
    <String Name="InvalidPlatformArchitecture">This version of the .NET Framework 2.0 is not supported on a 64-bit operating system. Contact your application vendor.</String>
    <String Name="WindowsInstallerImproperInstall">Due to an error with Windows Installer, the installation of the .NET Framework 2.0 cannot proceed.</String>
    <String Name="AnotherInstanceRunning">Another instance of setup is already running. The running instance must complete before this setup can proceed.</String>
    <String Name="BetaNDPFailure">A beta version of the .NET Framework was detected on the computer. Uninstall any previous beta versions of .NET Framework before continuing.</String>
    <String Name="GeneralFailure">A failure occurred attempting to install the .NET Framework 2.0.</String>
    <String Name="DotNetFXExe">http://go.microsoft.com/fwlink/?LinkId=37283</String>
    <String Name="InstMsiAExe">http://go.microsoft.com/fwlink/?LinkId=37285</String>
    <String Name="Msi30Exe">http://go.microsoft.com/fwlink/?LinkId=37287</String>
</Strings>
```

## <a name="see-also"></a>Weitere Informationen
- [\<Package> gewisses](../deployment/package-element-bootstrapper.md)