---
title: Microsoft Defenderi kasutamine Office 365 anti-phishing Policy
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693241"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Microsoft Defenderi kasutamine Office 365 anti-phishing Policy

Need sätted võimaldavad poliitika nimega *domeen ja tegevjuht*. See poliitika tagab nii kasutaja-kui ka domeeni kaitse ja rakendab seejärel poliitika kõigi domeenis kasutajate vastu võetud meilisõnumite kohta. Esmalt lisage poliitika loomiseks järgmine teave.

- **Nimi**: Domain and CEO **Kirjeldus**: tagab, et tegevjuht ja teie domeeni ei kehastata.
  **Rakendatud**: valige **adressaadi Domeen**. Valige **mõnest** jaotisest nupp **Vali** ja seejärel valige Domeen. Valige **+ Lisa**. Märkige loendis selle domeeni nimi (nt *contoso.com*) kõrval olev ruut ja seejärel valige **Lisa**. Valige **valmis**.
- Kui poliitika on loodud, saate poliitika viimistleda järgmiste suvandite abil.
  - **Kasutajate lisamine kaitsmiseks tehke järgmist.** Selles näites lisage tegevjuhi meiliaadress vähemalt.
  - **Domeenide lisamine, mida soovite kaitsta**: saate lisada ettevõtte tegevjuhti sisaldava domeeni.
  - Valige **toimingud**: meilisõnumi **saatmisel kehastanud kasutaja poolt** valige **suuna sõnum ümber teisele** meiliaadressile ja seejärel sisestage selle turvalisuse halduri meiliaadress (nt *securityadmin@contoso.com*). **Kui meilisõnumid saadetakse kehastava domeeni kaudu**, valige **sõnum karantiinis**.
  - **Postkasti luure**: Vaikimisi on see suvand valitud, kui loote uue andmepüügi poliitika. Jätke **see säte parimate** tulemuste saamiseks.
  - **Usaldusväärsete saatjate ja domeenide lisamine.** Selles näites ära Määratle ühtegi alistamist.
- Kui olete oma sätted üle vaadanud, valige **Loo see poliitika** või **Salvesta** vastavalt vajadusele.

Lisateavet leiate teemast [Microsoft 365 anti-andmepüügi poliitikad](https://go.microsoft.com/fwlink/?linkid=2092235).
