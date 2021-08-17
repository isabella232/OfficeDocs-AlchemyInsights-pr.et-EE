---
title: Uurige, kes on postkastis edasisaatmise häälestanud ja kuidas
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
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895175"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Uurige, kes on postkastis edasisaatmise häälestanud ja kuidas

Kui väline edasisuunamine on postkastis määratud, auditeeritakse tegevust **cmdlet-käsu Set-Mailbox osana.** Tegevuste leidmiseks auditilogist saate teha nii:

1. Tehke ühte järgmistest toimingutest.
   - Avage Microsoft 365 vastavuskeskus lahenduste audit <https://compliance.microsoft.com>  \> . Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://compliance.microsoft.com/auditlogsearch> .
   - Avage Microsoft 365 Defender portaalis <https://security.microsoft.com> **Audit**. Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://security.microsoft.com/auditlogsearch> .

   > [!NOTE]
   > Kui näete teadet, et peate auditeerimise sisse lülitama, lülitage see kohe sisse. Kui see funktsioon pole sisse lülitatud, ei saa otsingutulemid eelmistest kuupäevadest andmeid tõmmata.

2. Kontrollige **lehel** Audit, kas vahekaart **Otsing** on valitud, ja seejärel konfigureerige järgmised sätted.
   - Valige väljadele Algus ja Lõpp **kuupäeva-/kellaajavahemik.** 
   - Veenduge, **et väli Tegevused** **sisaldaks kõigi tegevuste tulemite kuvamist.**

3. Kui olete lõpetanud, klõpsake nuppu **Otsi**. Tegevused kuvatakse uuel lehel **Auditiotsing.**

4. Tulemite sortimiseks **klõpsake** tulemite sortimiseks veergu Tegevus ja otsige käsku **Sea postkastikirjed.**

5. Üksikasjade hüpiku avamiseks valige tulemitest soovitud tegevus. Selleks et teha kindlaks, kas tegevus on seotud meilisõnumite edasisaatmisega, peate vaatama iga auditikirje üksikasju.
   - **ObjectId**: muudetud postkasti pseudonüüm.
   - **Parameetrid:** _ForwardingSmtpAddress tähistab_ sihtmeiliaadressi.
   - **UserId**: Kasutaja, kes konfigureeris meilisõnumite edasisaatmise väljal **ObjectId olevas postkastis.**

Lisateavet leiate teemast [Postkasti jaoks meilisõnumite edasisaatmise häälestaja määratlemine.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
