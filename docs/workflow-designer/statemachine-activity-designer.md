---
title: Workflow-Designer-StateMachine-Aktivitäts Designer
description: Erfahren Sie, wie die StateMachine-Aktivität eine Auflistung von Zustands-und Modell Workflows mithilfe des vertrauten Zustands Automaten Paradigmas enthält.
ms.custom: SEO-VS-2020
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- StateMachine Designer
- System.Activities.Statements.StateMachine.UI
ms.assetid: 474d5fb3-1049-4b3f-bc6b-7524dbbe1672
ms.author: tglee
manager: jillfra
ms.workload:
- multiple
author: TerryGLee
ms.openlocfilehash: dacb6dfa5c30ce174c64accfedf82f1c288c734d
ms.sourcegitcommit: ed26b6e313b766c4d92764c303954e2385c6693e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/10/2020
ms.locfileid: "94433946"
---
# <a name="statemachine-activity-designer"></a>StateMachine-Aktivitäts-Designer

Die <xref:System.Activities.Statements.StateMachine>-Aktivität enthält eine Auflistung von Zustands- und Modellworkflows, die das bekannte Zustandsautomatenparadigma verwenden.

## <a name="using-the-statemachine-activity-designer"></a>Verwenden des StateMachine-Aktivitäts-Designers

Um eine- <xref:System.Activities.Statements.StateMachine> Aktivität hinzuzufügen, ziehen Sie den **StateMachine** -Aktivitäts-Designer aus dem Abschnitt **Zustands Automat** der **Toolbox** , und legen Sie ihn auf der Workflow-Designer Oberfläche ab. Um dieser Aktivität einen untergeordneten Zustand hinzuzufügen <xref:System.Activities.Statements.StateMachine> , ziehen <xref:System.Activities.Statements.State> Sie eine oder <xref:System.Activities.Core.Presentation.FinalState> aus der **Toolbox** , und legen Sie Sie auf dem **StateMachine** -Element ab.

### <a name="statemachine-activity-properties-in-the-workflow-designer"></a>Eigenschaften der StateMachine-Aktivität im Workflow-Designer

In der folgenden Tabelle sind die <xref:System.Activities.Statements.StateMachine>-Eigenschaften aufgeführt, die mithilfe des Workflow-Designers festgelegt werden können, und es wird beschrieben, wie sie im Designer verwendet werden. Diese Eigenschaften können im Eigenschaftenraster, einige davon auf der Designeroberfläche bearbeitet werden.

|Eigenschaftenname|Erforderlich|Verwendung|
|-|--------------|-|
|<xref:System.Activities.Activity.DisplayName%2A>|FALSE|Gibt den benutzerfreundlichen Namen der <xref:System.Activities.Statements.StateMachine>Aktivität im Header an. Der Standardwert ist **StateMachine**. Der Wert kann im Eigenschaftenraster oder direkt im Header des Aktivitätsdesigners bearbeitet werden. <xref:System.Activities.Activity.DisplayName%2A> wird in der Breadcrumbnavigation verwendet, die am oberen Rand des Workflow-Designers angezeigt wird.<br /><br /> Obwohl der <xref:System.Activities.Activity.DisplayName%2A> nicht zwingend erforderlich ist, wird empfohlen, einen Anzeigenamen zu verwenden.|

## <a name="see-also"></a>Siehe auch

- [Flussdiagramm](../workflow-designer/flowchart-activity-designer.md)
- [Ablaufsteuerung](../workflow-designer/control-flow-activity-designers.md)
