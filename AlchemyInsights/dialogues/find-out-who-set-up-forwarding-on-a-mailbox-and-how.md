---
title: Vaadake, kes häälestas postkastis edasisaatmise ja kuidas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429611"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Vaadake, kes häälestas postkastis edasisaatmise ja kuidas

Kui postkastis on määratud väline edasisaatmine, auditeeritakse tegevust Set-Mailbox cmdlet-käsu osana. Auditilogi tegevuse leidmiseks tehke järgmist.

1. Avage [Office 365 turbe & täitmise keskus](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Valige **Otsingu** >  **auditilogi otsing**.
    > [!NOTE]
    > Kui kuvatakse teade selle kohta, et teil on vaja auditit lülitada, jätkake ja lülitage see kohe välja. Kui see funktsioon pole sisse lülitatud, ei saa otsingutulemused eelmistest kuupäevadest andmeid tõmmata.
1. Veenduge, et välja **Tegevused** väärtuseks on seatud **kõigi tegevuste tulemid** (vaikeväärtus). Määrake kuupäevavahemik. Te ei pea kasutajanime määrama.
1. Valige **Otsi**. Tegevused kuvatakse jaotises **tulemid**.
1. Valige **Filtreeri tulemid** ja seejärel sisestage väljale **tegevuse** filter väärtus **Set-postkast** . See funktsioon annab tulemuseks kõik **postkasti** toimingud.
1. Üksikasjade kuvamiseks valige tegevus ja seejärel valige **rohkem teavet**. Jaotises **Parameetrid** saate vaadata postkastis määratud edasisaatmise meiliaadressi. **Kasutajanimi** tähistab kasutajat, kes häälestas postkastis välise edasisaatmise.
Lisateavet leiate teemast [Office 365 auditilogi otsimine levinud stsenaariumide tõrkeotsinguks](https://go.microsoft.com/fwlink/?linkid=2103944).