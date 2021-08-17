---
title: Sisendkausta reeglitegevuse tuvastamine auditilogides
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891291"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Sisendkausta reeglitegevuse tuvastamine auditilogides

Auditilogi otsingut saate kasutada Microsoft 365 vastavuskeskus sisendkausta reeglisündmuste (sisendkaustareeglite loomine, muutmine ja kustutamine) vaatamiseks.

1. Tehke ühte järgmistest toimingutest.
   - Avage Microsoft 365 vastavuskeskus lahenduste audit <https://compliance.microsoft.com>  \> . Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://compliance.microsoft.com/auditlogsearch> .
   - Avage Microsoft 365 Defender portaalis <https://security.microsoft.com> **Audit**. Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://security.microsoft.com/auditlogsearch> .

2. Konfigureerige  lehe **Audit vahekaardil Otsing** järgmised sätted.
   - **Kuupäeva- ja kellaajavahemik:** valige väljadele Algus ja Lõpp **kuupäeva-/kellaajavahemik.** 
   - **Tegevused:** valige üks või mitu järgmistest väärtustest.
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Sisendkaustareeglite värskendamine Outlook klientrakenduses**

3. Kui olete lõpetanud, klõpsake nuppu **Otsi**. Tegevused kuvatakse uuel lehel **Auditiotsing.**

4. Üksikasjade hüpiku avamiseks valige tulemitest soovitud tegevus. Teave sisendkausta reegli sätete kohta kuvatakse väljal **Parameetrid.**

Lisateavet leiate teemast Sisendkaustareegli [loomise kindlaksmääramine.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
