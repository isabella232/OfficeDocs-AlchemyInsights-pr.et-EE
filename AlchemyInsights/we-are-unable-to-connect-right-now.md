---
title: Aktiveerimisprobleem – me ei saa praegu ühendust luua
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806438"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 rakenduste parandamine sõnumis "Me ei saa praegu ühendust luua"

Kui teile kuvatakse see teade, proovige järgmist.

1. Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et veenduda, et need ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele. Vt [Microsofti URL-id ja IP-aadresside vahemikud.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Avage Start Run  >  **(Käivita)** ja seejärel tippige **services.msc**. Veenduge, et kõik järgmised teenused töötaks.
    - Võrguühendusega seadmete automaathäälestus
    - Võrguteenus
    - Võrguasukoha teadlikkus
    - Windowsi sündmuste logi

Kui mõni neist teenustest ei tööta, proovige seda käivitada. Kui teil on teenuse käivitamisel probleeme, käivitage järgmine käsk, avades administraatoriõigustega käsuviiba.

**sfc /scannow**

Pärast selle käsu lõpule viimist taaskäivitage arvuti.

Üksikasjalikku teavet leiate teemast ["Kahjuks ei saa me teie kontoga ühendust luua. Proovige hiljem uuesti", kui aktiveerite Office'i Microsoft 365-st.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)