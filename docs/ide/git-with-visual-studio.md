---
title: Git-Benutzeroberfläche in Visual Studio
titleSuffix: ''
description: In diesem Artikel erfahren Sie, wie Sie mithilfe der neuen integrierten Git-Benutzeroberfläche in Visual Studio 2019 Ihre Produktivität steigern können.
ms.date: 11/16/2020
ms.topic: conceptual
ms.author: tglee
author: TerryGLee
ms.manager: jillfra
monikerRange: vs-2019
ms.openlocfilehash: 30ae69f07c89efb6d01228088596fc1bc05fac87
ms.sourcegitcommit: e8a13978131f257d91ce37c5a2e0d153a4c400ef
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2020
ms.locfileid: "94704065"
---
# <a name="git-experience-in-visual-studio"></a>Git-Benutzeroberfläche in Visual Studio

Git ist nun die Standardressource für die Versionskontrolle in Visual Studio 2019. Seit [Version 16.6](/visualstudio/releases/2019/release-notes-v16.6) wurde das Featurespektrum anhand des Benutzerfeedbacks weiter ausgearbeitet und verbessert. Die neue Git-Benutzeroberfläche ist seit dem Release von [Version 16.8](/visualstudio/releases/2019/release-notes/) standardmäßig für alle Benutzer aktiviert.

> [!TIP]
> Git ist das am häufigsten verwendete moderne Versionskontrollsystem. Unabhängig davon, ob Sie ein professioneller Entwickler sind oder erst die Grundlagen des Programmierens erlernen, kann Git sehr nützlich für Sie sein. Wenn Sie noch nicht mit Git vertraut sind, ist die Website https://git-scm.com/ ein guter Startpunkt. Dort finden Sie Spickzettel, ein beliebtes E-Book sowie Videos zu den Git-Grundlagen.

## <a name="how-to-use-git-in-visual-studio"></a>Verwenden von Git in Visual Studio

In diesem Artikel erhalten Sie eine detaillierte Anleitung zur Verwendung der neuen Git-Benutzeroberfläche in Visual Studio 2019. Wenn Sie jedoch vorab bereits einen kurzen Blick darauf werfen möchten, können Sie sich das folgende Video ansehen: <br><br>*Länge des Videos: 5,27 Minuten*

> [!VIDEO https://www.youtube.com/embed/UHrAg3iKoe0]

Es gibt drei Möglichkeiten, Ihre Produktivität mit Git in Visual Studio zu steigern:

- [Öffnen eines vorhandenen Git-Repositorys:](#open-an-existing-local-repository) Wenn sich Ihr Code bereits auf Ihrem Computer befindet, können Sie ihn über **Datei** > **Öffnen** > **Projekt/Projektmappe** (oder **Ordner**) öffnen. Visual Studio erkennt automatisch, ob ein initialisiertes Git-Repository verfügbar ist.
- [Erstellen eines neuen Git-Repositorys:](#create-a-new-git-repository) Wenn Ihr Code Git nicht zugeordnet ist, können Sie ein neues Git-Repository erstellen.
- [Klonen eines vorhandenen Git-Repositorys:](#clone-an-existing-git-repository) Wenn sich der Code, mit dem Sie arbeiten möchten, nicht auf Ihrem Computer befindet, können Sie jedes beliebige Remoterepository klonen.

> [!NOTE]
> Ebenfalls ab [Version 16.8](/visualstudio/releases/2019/release-notes/) steht Ihnen in Visual Studio 2019 eine vollständig integrierte GitHub-Kontobenutzeroberfläche zur Verfügung. Sie können Ihrer Keychain nun sowohl GitHub- als auch GitHub Enterprise-Konten hinzufügen. Sie können sie genauso wie Microsoft-Konten hinzufügen und nutzen. Dies vereinfacht den Zugriff auf GitHub-Ressourcen in Visual Studio für Sie. Weitere Informationen finden Sie auf der Seite [Arbeiten mit GitHub-Konten in Visual Studio](work-with-github-accounts.md).

## <a name="create-a-new-git-repository"></a>Erstellen eines neuen Git-Repositorys

Wenn Ihr Code Git nicht zugeordnet ist, können Sie zunächst ein neues Git-Repository erstellen. Klicken Sie hierzu in der Menüleiste auf **Git** > **Git-Repository erstellen**. Geben Sie dann in im Dialogfeld **Neues Git-Repository erstellen** Ihre Informationen ein.

:::image type="content" source="media/git-create-repository.png" alt-text="Screenshot: Dialogfeld „Git-Repository erstellen“ in Visual Studio":::

Durch das Dialogfeld **Git-Repository erstellen** können Sie Ihr neues Repository einfach mithilfe von Push an GitHub übertragen. Ihr neues Repository ist standardmäßig privat. Dies bedeutet, dass Sie die einzige Person sind, die darauf zugreifen kann. Wenn Sie das Kontrollkästchen deaktivieren, ist Ihr Repository öffentlich, sodass es von jedem auf GitHub angezeigt werden kann.

> [!TIP]
> Unabhängig davon, ob Ihr Repository privat oder öffentlich ist, ist es am besten, über eine auf GitHub gespeicherte Remotesicherung Ihres Codes zu verfügen, auch wenn Sie nicht mit einem Team zusammenarbeiten. Dies macht Ihren Code auch für Sie verfügbar, unabhängig davon, welchen Computer Sie verwenden.

Sie können ein lokales Git-Repository erstellen, indem Sie die Option **Nur lokal** verwenden. Alternativ können Sie Ihr Repository über die Option **Existing remote** (Vorhandenes Remoterepository) mit einem vorhandenen leeren Remoterepository auf einem beliebigen anderen Git-Anbieter verknüpfen.

## <a name="clone-an-existing-git-repository"></a>Klonen eines vorhandenen Git-Repositorys

Visual Studio bietet eine direkte Funktion zum Klonen. Wenn Sie die URL des Repositorys kennen, das Sie klonen möchten, können Sie die URL im Abschnitt **Repositoryspeicherort** einfügen und dann den Speicherort auf dem Datenträger auswählen, an dem Visual Studio das Repository klonen soll.

:::image type="content" source="media/git-clone-repository.png" alt-text="Screenshot: Dialogfeld „Repository klonen“ in Visual Studio":::

Wenn Sie die Repository-URL nicht kennen, können Sie mit Visual Studio problemlos Ihr vorhandenes GitHub- oder Azure DevOps-Repository suchen und anschließend klonen.

### <a name="open-an-existing-local-repository"></a>Öffnen eines vorhandenen lokalen Repositorys

Nachdem Sie ein Repository geklont oder eines erstellt haben, erkennt Visual Studio das Git-Repository und fügt es der Liste der **Local Repositories** (Lokale Repositorys) im Git-Menü hinzu. Von hier aus können Sie schnell auf Ihre Git-Repositorys zugreifen oder zwischen diesen wechseln.

:::image type="content" source="media/git-local-repositories.png" alt-text="Screenshot: Option „Local Repositories“ (Lokale Repositorys) im Git-Menü in Visual Studio":::

## <a name="view-files-in-solution-explorer"></a>Anzeigen von Dateien im Projektmappen-Explorer

Wenn Sie ein Repository klonen oder ein lokales Repository öffnen, wechselt Visual Studio in diesen Git-Kontext, indem alle zuvor geöffneten Lösungen und Projekte gespeichert und geschlossen werden. Der Projektmappen-Explorer lädt den Ordner im Stammverzeichnis des Git-Repositorys und scannt die Verzeichnisstruktur auf beliebige Ansichtsdateien. Hierzu gehören Dateien wie „CMakeLists.txt“ oder solche mit der Dateierweiterung „.sln“.

Visual Studio passt die Ansicht an, je nachdem, welche Ansichtsdatei Sie im Projektmappen-Explorer laden:

- Wenn Sie ein Repository klonen, das eine einzelne SLN-Datei enthält, lädt der Projektmappen-Explorer diese Lösung direkt für Sie.
- Wenn der Projektmappen-Explorer keine SLN-Dateien in Ihrem Repository erkennt, wird standardmäßig die Ordneransicht geladen.
- Wenn Ihr Repository mehr als eine SLN-Datei enthält, zeigt der Projektmappen-Explorer die Liste der verfügbaren Ansichten an, aus denen Sie eine auswählen können.

Sie können mithilfe der Schaltfläche **Ansicht umschalten** auf der Symbolleiste des Projektmappen-Explorers zwischen der aktuell geöffneten Ansicht und den Optionen in der Liste der Ansichten wechseln.

:::image type="content" source="media/git-solution-explorer-views.png" alt-text="Screenshot: Ausgewählte Projektmappen-Explorer-Option „Ansicht umschalten“ in Visual Studio":::

## <a name="git-changes-window"></a>Fenster „Git-Änderungen“

Git verfolgt Dateiänderungen in Ihrem Repository, während Sie arbeiten, und unterteilt die Dateien in Ihrem Repository in drei Kategorien. Diese Änderungen sind gleichbedeutend mit dem, was Sie sehen, wenn Sie den Befehl `git status` in der Befehlszeile eingeben:

- **Unveränderte Dateien:** Diese Dateien wurden seit dem letzten Commit nicht geändert.
- **Geänderte Dateien:** Diese Dateien weisen Änderungen seit dem letzten Commit auf, aber Sie haben sie noch nicht für den nächsten Commit gestaget.
- **Gestagete Dateien:** Diese Dateien weisen Änderungen auf, die mit dem nächsten Commit hinzugefügt werden.

Während Ihrer Arbeit werden Änderungen an Dateien in Ihrem Projekt von Visual Studio im Abschnitt **Änderungen** des Fensters **Git-Änderungen** nachverfolgt.

:::image type="content" source="media/git-changes-window.png" alt-text="Screenshot: Fenster „Git-Änderungen“ in Visual Studio":::

Wenn Sie bereit sind, Änderungen zu stagen, klicken Sie für jede zu stagende Datei auf die Schaltfläche **+** (Pluszeichen). Alternativ können Sie mit der rechten Maustaste auf eine Datei und dann auf **Stufe** klicken. Sie können auch alle geänderten Dateien mit einem Mausklick stagen, indem Sie die Schaltfläche **+** (Pluszeichen) oben im Abschnitt **Änderungen** zum Stagen aller Dateien verwenden.

Wenn Sie eine Änderung stagen, erstellt Visual Studio den Abschnitt **Gestagete Änderungen**. Nur Änderungen im Abschnitt **Gestagete Änderungen** werden beim nächsten Commit hinzugefügt. Klicken Sie hierzu auf **Gestageter Commit**. Sie können Änderungen auch unstagen, indem Sie auf die Schaltfläche **–** (Minuszeichen) klicken. Der entsprechende Befehl für diese Aktion ist `git commit -m "Your commit message"`.

Sie können sich auch dazu entscheiden, Ihre geänderten Dateien nicht zu stagen, indem Sie den Stagingbereich überspringen. In diesem Fall ermöglicht Visual Studio das Committen Ihrer Änderungen direkt ohne Staging. Geben Sie einfach Ihre Commitnachricht ein, und klicken Sie auf **Alle committen**. Der entsprechende Befehl für diese Aktion ist `git commit -a`.

Visual Studio erleichtert mithilfe der Verknüpfungen **Commit für alle und Push** und **Commit für alle und Sync** auch das Committen und Synchronisieren mit nur einem Mausklick. Wenn Sie in den Abschnitten **Änderungen** und **Gestagete Änderungen** auf eine beliebige Datei doppelklicken, wird ein zeilenweiser Vergleich mit der nicht geänderten Version der Datei angezeigt.

:::image type="content" source="media/git-file-version-compare.png" alt-text="Screenshot: Zeilenweiser Vergleich der Dateiversionen in Visual Studio":::

> [!TIP]
> Wenn Sie eine Verbindung mit dem Azure DevOps-Repository hergestellt haben, können Sie ein Azure DevOps-Arbeitselement mithilfe des Zeichens „#“ committen. Sie können Ihr Azure DevOps-Repository über **Team Explorer** > **Verbindungen verwalten** verbinden.

### <a name="select-an-existing-branch"></a>Auswählen eines vorhandenen Branchs

Visual Studio zeigt den aktuellen Branch im Selektor am oberen Rand des Fensters **Git-Änderungen** an.

:::image type="content" source="media/git-changes-current-branch-selector.png" alt-text="Screenshot: Aktueller Branch, der über den Selektor am oberen Rand des Fensters „Git-Änderungen“ in Visual Studio angezeigt werden kann":::

Der aktuelle Branch ist auch auf der Statusleiste in der rechten unteren Ecke der Visual Studio-IDE verfügbar.

:::image type="content" source="media/git-changes-current-branch-status-bar.png" alt-text="Screenshot: Aktuelle Branches, die mithilfe der Statusleiste in der unteren rechten Ecke in der Visual Studio-IDE angezeigt werden können":::

An beiden Speicherorten können Sie zwischen vorhandenen Branches wechseln.

### <a name="create-a-new-branch"></a>Neuen Branch erstellen

Sie können auch einen neuen Branch erstellen. Der entsprechende Befehl für diese Aktion ist `git checkout <branchname>`.

Das Erstellen eines neuen Branchs ist so einfach wie das Eingeben des Branchnamens und Verwenden eines vorhandenen Branchs als Basis.

:::image type="content" source="media/git-changes-create-new-branch.png" alt-text="Screenshot: Dialogfeld „Neuen Branch erstellen“ in Visual Studio":::

Sie können einen vorhandenen lokalen Branch oder einen Remotebranch als Basis verwenden. Das Kontrollkästchen **Branch auschecken** leitet Sie automatisch zum neu erstellten Branch weiter. Der entsprechende Befehl für diese Aktion ist `git checkout -b <new-branch><existing-branch>`.

## <a name="git-repository-window"></a>Fenster „Git-Repository“

Visual Studio verfügt über das neue Fenster **Git-Repository**, bei dem es sich um eine konsolidierte Ansicht aller Details in Ihrem Repository einschließlich aller Verläufe in Bezug auf Branches, Remoterepositorys und Commits handelt. Sie können entweder über die Optionen **Git** oder **Ansicht** auf der Menüleiste oder über die Statusleiste direkt auf dieses Fenster zugreifen.

### <a name="manage-branches"></a>Verwalten von Branches

Wenn Sie im Menü **Git** auf **Branches verwalten** klicken, wird im Fenster **Git-Repository** die Branchstrukturansicht angezeigt. Im linken Bereich können Sie das Kontextmenü (Klick mit der rechten Maustaste) unter anderem verwenden, um Branches zu überprüfen, neue Branches zu erstellen oder diese zusammenzuführen. Außerdem können Sie Rebases und Cherry-Picks ausführen. Wenn Sie auf den Branch klicken, wird im rechten Bereich eine Vorschau des zugehörigen Commitverlaufs angezeigt.

### <a name="incoming-and-outgoing-commits"></a>Eingehende und ausgehende Commits

Wenn Sie einen Branch fetchen, verfügt das Fenster **Git-Änderungen** unter dem Dropdownmenü für den Branch über einen Indikator, der die Anzahl nicht gepullter Commits aus dem Remotebranch anzeigt. Dieser Indikator zeigt außerdem die Anzahl der nicht mithilfe von Push übertragenen lokalen Commits an.

:::image type="content" source="media/git-repo-drop-down-indicator.png" alt-text="Screenshot: Fenster „Git-Changes“ mit dem Benutzeroberflächenelement für das Indikatordropdownmenü in Visual Studio":::

Der Indikator fungiert auch als Verlinkung zum Commitverlauf des Branchs im Fenster **Git-Repository**. Oben im Verlauf werden nun die Details dieser eingehenden und ausgehenden Commits angezeigt. Von hier aus können Sie die Commits auch pullen oder mithilfe von Push übertragen.

:::image type="content" source="media/git-branch-commit-history.png" alt-text="Screenshot: Fenster „Git-Repository“ mit dem Commitverlauf eines Branchs in Visual Studio":::

#### <a name="commit-details"></a>Commitdetails

Wenn Sie auf einen **Commit** doppelklicken, zeigt Visual Studio die entsprechenden Details in einem separaten Toolfenster an. Von hier aus können Sie den Commit rückgängig machen, zurücksetzen, die Commitnachricht ändern oder ein Tag für den Commit erstellen. Wenn Sie auf eine geänderte Datei im Commit klicken, öffnet Visual Studio die parallele **Diff**-Ansicht des Commits und des übergeordneten Elements.

:::image type="content" source="media/git-branch-commit-details.png" alt-text="Screenshot: Dialogfeld „Commitdetails“ in Visual Studio":::

## <a name="handle-merge-conflicts"></a>Behandeln von Mergekonflikten

Während eines Mergevorgangs können Konflikte auftreten, wenn zwei Entwickler die gleichen Zeilen in einer Datei ändern und Git nicht automatisch weiß, welche Zeile korrekt ist. Git hält den Merge an und informiert Sie darüber, dass ein Konflikt besteht.

Visual Studio erleichtert das Identifizieren und Lösen von Mergekonflikten. Zuerst zeigt das Fenster **Git-Repository** am oberen Rand eine goldene Infoleiste an.

:::image type="content" source="media/git-merge-conflict-gold-bar.png" alt-text="Screenshot: Meldung &quot;Der Merge in Repository (...) wurde mit Konflikten abgeschlossen.&quot; in Visual Studio":::

Das Fenster **Git-Änderungen** zeigt auch die Meldung *"Merge wird mit Konflikten ausgeführt."* mit den nicht gemergten Dateien in einem separaten Abschnitt darunter an.

:::image type="content" source="media/git-merge-progress-conflicts-message.png" alt-text="Screenshot: Meldung &quot;Merge wird mit Konflikten ausgeführt.&quot; in Visual Studio":::

Wenn keines dieser Fenster geöffnet ist und Sie stattdessen zu der Datei mit Mergekonflikten navigieren, müssen Sie nicht nach dem folgenden Text suchen:

```bash
    <<<<<<< HEAD
    =======
    >>>>>>> main
```

Stattdessen zeigt Visual Studio oben auf der Seite eine goldene Infoleiste an, die angibt, dass im Zusammenhang mit der geöffneten Datei Konflikte bestehen. Anschließend können Sie auf die Verlinkung klicken, um den **Merge-Editor** zu öffnen.

:::image type="content" source="media/git-merge-conflict-gold-info-bar.png" alt-text="Screenshot: Meldung &quot;File contains merge conflicts.&quot; (Im Zusammenhang mit dieser Datei bestehen Mergekonflikte.) in Visual Studio":::

### <a name="the-merge-editor"></a>Merge-Editor

Der Merge-Editor in Visual Studio ist ein Drei-Wege-Mergetool, das die eingehenden Änderungen, die aktuellen Änderungen und das Ergebnis des Merges anzeigt. Sie können die Symbolleiste oben im **Merge-Editor** verwenden, um zwischen Konflikten und automatisch gemergten Unterschieden in der Datei zu navigieren.

:::image type="content" source="media/git-merge-editor.png" alt-text="Screenshot: Merge-Editor in Visual Studio":::

Sie können auch die Umschaltflächen zum Anzeigen bzw. Ausblenden von Unterschieden und Wortunterschieden oder das Anpassen des Layouts verwenden. Oben auf jeder Seite befinden sich Kontrollkästchen, die Sie verwenden können, um alle Änderungen von der einen Seite für die andere Seite zu übernehmen. Wenn Sie jedoch einzelne Änderungen vornehmen möchten, können Sie auf beiden Seiten auf die Kontrollkästchen links neben den in Konflikt stehenden Zeilen klicken. Wenn Sie schließlich die Konflikte beseitigt haben, können Sie im Merge-Editor auf die Schaltfläche **Merge akzeptieren** klicken. Anschließend schreiben Sie eine Commitnachricht und committen die Änderungen, um den Vorgang abzuschließen.

## <a name="personalize-your-git-settings"></a>Personalisieren der Git-Einstellungen

Navigieren Sie auf der Menüleiste entweder zu **Git** > **Einstellungen** oder zu **Extras** > **Optionen** > **Quellcodeverwaltung**, um Ihre Git-Einstellungen sowohl auf Repositoryebene als auch auf globaler Ebene zu personalisieren und anzupassen. Wählen Sie anschließend die gewünschten Optionen aus.

:::image type="content" source="media/git-options-settings.png" alt-text="Screenshot: Dialogfeld „Optionen“ zum Personalisieren und Anpassen von Einstellungen in der Visual Studio-IDE":::

## <a name="how-to-use-the-legacy-team-explorer-experience-in-visual-studio"></a>Verwenden der Legacyversion des Team Explorers in Visual Studio

Die neue Git-Benutzeroberfläche stellt ab [Version 16.8](/visualstudio/releases/2019/release-notes/) das Standardsystem für die Versionskontrolle in Visual Studio 2019 bereit. Wenn Sie sie deaktivieren möchten, können Sie dies jedoch auch tun. Wechseln Sie zu **Extras** > **Optionen** > **Umgebung** > **Vorschaufeatures**, und aktivieren Sie das Kontrollkästchen **New Git user experience** (Neue Git-Benutzeroberfläche), wodurch Sie zur Legacyversion des Team Explorers zurückkehren.

:::image type="content" source="media/git-opt-new-user-experience.png" alt-text="Screenshot: Abschnitt „Vorschaufeatures“ des Dialogfelds „Optionen“ in Visual Studio":::

## <a name="whats-next"></a>Nächste Schritte

Die neue Git-Benutzeroberfläche ist in Visual Studio 2019, [Version 16.8](/visualstudio/releases/2019/release-notes/), zwar standardmäßig aktiviert, wird aber weiterhin um neue Features erweitert, um die Leistung zu verbessern. Wenn Sie neue Updates der Git-Benutzeroberfläche in einem Vorschaurelease ausprobieren möchten, können Sie diese über die Seite [Visual Studio Preview](https://aka.ms/vspreview/) herunterladen und installieren.

> [!IMPORTANT]
> Wenn Sie einen Vorschlag haben, können Sie uns diesen gerne mitteilen. Wir freuen uns, Entwurfsentscheidungen im Portal für die [**Entwicklercommunity**](https://aka.ms/vs-suggest) diskutieren zu können.

## <a name="see-also"></a>Weitere Informationen

- Blogbeitrag [Ankündigung der Git-Benutzeroberfläche in Visual Studio](https://devblogs.microsoft.com/visualstudio/announcing-the-release-of-the-git-experience-in-visual-studio/)
- [Start der neuen Git-Benutzeroberfläche](https://www.youtube.com/watch?v=UHrAg3iKoe0&t) auf YouTube
- [Die Serie „Visual Studio Toolbox“ präsentiert: The new Git experience](https://channel9.msdn.com/Shows/Visual-Studio-Toolbox/The-New-Git-Experience) (Die neue Git-Benutzeroberfläche) auf Channel 9 und auf [YouTube](https://www.youtube.com/watch?v=ZiQ2LXtAJ6I&feature=youtu.be)
- Blogbeitrag zu den [aufregenden neuen Updates in Bezug auf die Git-Benutzeroberfläche in Visual Studio](https://devblogs.microsoft.com/visualstudio/exciting-new-updates-to-the-git-experience-in-visual-studio/)
- Blogbeitrag zur [verbesserten Git-Benutzeroberfläche in Visual Studio 2019](https://devblogs.microsoft.com/visualstudio/improved-git-experience-in-visual-studio-2019/)
- [Arbeiten mit GitHub-Konten in Visual Studio](work-with-github-accounts.md)
- [Visual Studio 2019 – Versionshinweise](/visualstudio/releases/2019/release-notes)
