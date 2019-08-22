---
title: Sisendkausta reegli tegevuse auditilogid tuvastada
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539160"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Sisendkausta reegli tegevuse auditilogid tuvastada

Office 365 turvalisuse & vastavuse Center auditi logifaili Otsi saate vaadata sisendkausta reegel sündmused (luua, muuta ja kustutada sisendkausta reeglid).

1. Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/).

2. Mine **Otsi** > **auditi logifaili** otsingulehte.

3. Valige kuupäevavahemik väljadele **Alguskuupäev** ja **lõppkuupäev** .

4. Kontrollige jaotises **Exchange'i postkasti tegevust**, **tegevuse** väärtuseks on **New-InboxRule loomine/muutmine/luba/Keela reegel**.

5. Klõpsake nuppu **Otsi**.

Tulemused, valige audit kirje. Hüpik üksikasjad nuppu **Lisateave**. Sisendkausta reegli sätete kohta teabe kuvatakse väljal **Parameetrid** .

Lisateabe saamiseks vt [Determining kui sisendkausta reegel loonud kasutaja](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
