---
title: Sisendkausta reegli tegevuse auditilogid tuvastada
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417243"
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
