---
title: Microsoft 365 rakenduste parandamine Ei leidnud office'i litsentsidega seotud sõnumit
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816484"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Microsoft 365 rakenduste parandamine sõnumiga "Ei leidnud seotud office'i litsentse"

Kui teile kuvatakse see teade, proovige järgmist.

1. Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et veenduda, et need ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele. Vt [Microsoft 365 URL-id ja IP-aadresside vahemikud.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Eemaldage [mõjutatud kasutaja Office'i litsents](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja määrake see ümber. 
3. Avage Office'i rakendus [ja logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mis tahes olemasolevast kasutajakontost.
4. Avage Windowsi sätted >   >  **Meilikontod & kontod** ja eemaldage kõik töökontod peale mõjutatud konto.
5. Avage Windowsi sätted >   >  **Kontod Accessi töö- või koolikonto** ja katkestage ühendus kõigi töökontodega, v.a mõjutatud konto.
6. Lähtestage Office'i aktiveerimisolekut. [Vaadake, kuidas](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logige sisse](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mõjutatud kasutajakontoga.

Lisateavet tõrkeotsingulahenduste kohta leiate teemast [Litsentsimata toote- ja aktiveerimistõrked Office's.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)