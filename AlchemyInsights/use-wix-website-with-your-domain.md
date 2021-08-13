---
title: Wix-i veebisaidi kasutamine Office 365 või hallatavate domeenidega
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980173"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Wix-i veebisaidi kasutamine Office 365 või hallatavate domeenidega

- [Värskendage DNS-i kirjeid, et hoida oma veebisaiti praeguse majutusteenuse pakkuja juures](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix-artiklis "Domeeni ühendamine Wix-iga osutamismeetodi abil" soovitatakse kasutada osutamist (dns-i kirjete lisamine ülaltoodud lingi kohta) nimeserverite muutmise asemel Office 365
- Kui otsustate endiselt muuta nimeserverid Wix-iks, peate microsofti jaoks  [wix-is dns-i kirjeid looma.](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Kui teie domeen on ostetud Microsoftilt, ei saa nimeservereid muuta. Kui peate nimeservereid muutma, tuleb Microsofti ostetud domeen 60 päeva pärast üle viia  [teisele hostiteenuse pakkujale.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)