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
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755034"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Sisendkausta reegli tegevuse auditilogid tuvastada

Saate auditi Logi otsing turvalisuse & vastavuse Center sisendkausta reegel sündmuste (luua, muuta ja kustutada sisendkaustareeglid) vaatamiseks.

1. Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/)

2. Valige **Auditi logifaili Otsi**nuppu **Otsi ja uurimine** .

3. Valige kuupäevavahemik väljadele **Alguskuupäev** ja **lõppkuupäev** .

4. Kontrollige jaotises **Exchange'i postkasti tegevust**, **tegevuse** väärtuseks on **New-InboxRule loomine/muutmine/luba/Keela reegel**.

5. Klõpsake nuppu **Otsi**.

Tulemused, valige audit kirje. Hüpik üksikasjad nuppu **Lisateave**. Sisendkausta reegli sätete kohta teabe kuvatakse väljal **Parameetrid** .

Lisateabe saamiseks vt [Determining kui sisendkausta reegel loonud kasutaja](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
