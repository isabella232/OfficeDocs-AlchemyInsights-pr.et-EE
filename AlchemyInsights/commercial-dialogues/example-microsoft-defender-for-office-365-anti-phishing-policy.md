---
title: Microsoft Defenderi näide Office 365 andmepüügitõrje poliitika jaoks
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035002"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Microsoft Defenderi näide Office 365 andmepüügitõrje poliitika jaoks

Need sätted võimaldavad poliitika nimega *Domeen ja ceo*. See poliitika pakub nii kasutaja- kui ka domeenikaitset isikustamise eest ja rakendab seejärel poliitika kõigile domeeni kasutajatele vastu võetud meilisõnumitele. Esmalt lisage poliitika loomiseks järgmine teave.

- **Nimi**: Domain and CEO **Description**: Tagab, et ceo ja teie domeeni ei esineks kehastus.
  **Rakendus:** valige **Adressaadi domeen on**. Valige **jaotises Mõni neist** nupp **Vali** ja seejärel valige domeen. Valige **+ Lisa**. Märkige loendis domeeni nime (nt contoso.com *)* kõrval ruut **.** Valige **Valmis**.
- Pärast poliitika loomist saate poliitika viimistlemiseks kasutada järgmisi suvandeid.
  - **Kasutajate lisamine kaitsmiseks.** Selles näites lisage vähemalt ceo meiliaadress.
  - **Domeenide lisamine kaitsmiseks:** lisage ettevõtte domeen, mis sisaldab tegevjuhi kontorit.
  - **Valige toimingud.** **Kui** meilisõnumi on saatnud jäljendatud kasutaja , valige Suuna sõnum ümber teisele meiliaadressile ja sisestage turbeadministraatori meiliaadress *(nt securityadmin@contoso.com).* Kui **meilisõnumi on saatnud impersoneeritud** domeen, valige Pane sõnum **karantiini.**
  - **Postkasti jälitusteave.** Vaikimisi valitakse see suvand uue andmepüügitõrjepoliitika loomisel. Jätke see säte **parimate tulemuste saamiseks** sisse.
  - **Lisage usaldusväärseid saatjaid ja domeene.** Selles näites ärge määratlege ühtegi alistamist.
- Kui olete sätted läbi vaadanud, valige **vastavalt vajadusele** Käsk Loo see poliitika **või** Salvesta.

Lisateavet leiate teemast [Andmepüügivastased poliitikad Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
