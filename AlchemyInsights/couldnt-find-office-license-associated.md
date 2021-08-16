---
title: Rakenduste Microsoft 365 ei leidnud seotud office'i litsentse
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
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069600"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Sõnumi Microsoft 365 "Ei leidnud seotud office'i litsentse" parandamine

Kui teile kuvatakse see teade, proovige järgmist.

1. Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et veenduda, et need ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele. Vt [Microsoft 365 URL-id ja IP-aadresside vahemikud.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Eemaldage [ja määrake Office kasutaja](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) litsents ümber. 
3. Avage Office'i telefonirakendus [ja logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mis tahes olemasolevatest kasutajakontodelt.
4. Avage Windows Sätted >   >  **Meilikontod & kontod** ja eemaldage kõik töökontod, v.a mõjutatud konto.
5. Avage Windows Sätted >   >  **Kontod Accessi töö- või koolikonto** ja katkestage ühendus kõigi töökontodega, v.a mõjutatud konto.
6. Lähtestage Office aktiveerimisolekut. [Vaadake, kuidas](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logige sisse](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mõjutatud kasutajakontoga.

Lisateavet tõrkeotsingulahenduste kohta leiate teemast [Litsentsimata toote- ja aktiveerimistõrked Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).