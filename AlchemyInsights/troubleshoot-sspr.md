---
title: SSPR tõrkeotsing
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429722"
---
# <a name="troubleshoot-sspr"></a>SSPR tõrkeotsing

**Mul on probleeme parooli lähtestamise konfigureerimisega**

- Kui olete administraator ja otsite, kuidas lubada iseteeninduskeskuse parooli lähtestamist, lugege artiklit [õpetuse lubamine SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), et konfigureerida oma asutuse parooli lähtestamine. Võib-olla soovite ka [litsentsimise nõuded](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)üle vaadata. Teil peab olema vähemalt ühe ettevõttes määratud litsents.
    - **Ainult pilveteenuse kasutajad** – kõik Office 365 (O365) makstud SKU või Azure AD ' i põhifunktsioonid
    - **Pilv ja/või kohapealsed kasutajad** – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure produktiivne Enterprise (SPE)
- Lisateavet iseteeninduse parooli lähtestamise kohta leiate [meie KKK](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)-s.

**Kuvatakse tõrketeade**

Vaadake seda artiklit, et leida levinud tõrked ja nende lahendused: [iseteeninduskeskuse parooli lähtestamise tõrkeotsing](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mul on parooli lähtestamise poliitikaga probleeme**

- Kui teie parooli lähtestamise poliitika ei käitu ootuspäraselt või kui teil on küsimusi parooli lähtestamise poliitika kohta, vaadake seda artiklit: [Azure Active Directory parooliga seotud reeglid ja piirangud](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Parooli lähtestamise poliitika ei rakendu administraatoritele. Microsoft jõustab iga Azure ' i administraatori rolli jaoks tugeva vaike-kahe värava parooli lähtestamise poliitika. Veenduge, et katsetate kasutajaga, kes pole administraator. Lisateavet administraatori lähtestamise poliitika kohta leiate sellest artiklist: [administraatori lähtestamise poliitika erinevused](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Ma ei soovi, et kasutajad registreeriks parooli lähtestamiseks täiendava turbeteabe**

Saate oma kasutajatele API, PowerShelli või Azure AD Connecti kaudu andmeid (meili ja telefoni atribuudid) eelnevalt asustada. Lugege, kuidas lugeda:

- [Parooli lähtestamise juurutamine, mis ei nõua kasutajatelt registreerumist](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Milliseid andmeid parooli lähtestamine kasutab?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Soovin, et kasutajad registreeriks parooli lähtestamiseks täiendava turbeteabe**

1. Kas teie kasutajad registreerivad ise oma turbeteabe parooli lähtestamiseks, suunates need [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Kui kasutaja (kasutaja või administraator) on andmed asustanud, suunatakse kasutaja [aka.MS/SSPR](https://passwordreset.microsoftonline.com/) , et kasutajad saaksid oma paroole lähtestada.
1. Kui kasutajatel esineb endiselt probleeme, on need tõenäoliselt **ühendatud** või **parool Hash sünkroonitud** kasutajad. See tähendab, et tõenäoliselt esineb probleeme parooliga tagasikirjutusega teenusega.