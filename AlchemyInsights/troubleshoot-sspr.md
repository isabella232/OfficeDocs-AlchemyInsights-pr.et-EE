---
title: SSPR-i tõrkeotsing
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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038954"
---
# <a name="troubleshoot-sspr"></a>SSPR-i tõrkeotsing

**Mul on probleeme parooli lähtestamise konfigureerimisega**

- Kui olete administraator ja otsite iseteeninduse parooli lähtestamise lubamist, lugege teemat [SSPR-i](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)lubamine , et konfigureerida oma asutuse jaoks parooli lähtestamine. Samuti võite soovida [litsentsimisnõuded läbi vaadata.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Teie ettevõttes peab olema määratud vähemalt üks litsents.
    - **Ainult pilveteenuse kasutajad** – Office 365 (O365) tasuline SKU või Azure AD Basic
    - **Pilveteenuse ja/või kohapealne** kasutaja – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure Productive Enterprise (SPE)
- Lisateavet iseteeninduse parooli lähtestamise kohta vaadake [meie KKK-st.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Kuvatakse tõrketeade**

Levinumate tõrgete ja nende lahenduste leidmiseks vaadake seda artiklit. [Iseteeninduse parooli lähtestamise tõrkeotsing](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mul on probleem parooli lähtestamise poliitikaga**

- Kui teie paroolilähtestuspoliitika ei käitu ootuspäraselt või kui teil on küsimusi parooli lähtestamise poliitikate kohta, vaadake järgmist artiklit: Paroolipoliitikad [ja Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Parooli lähtestamise poliitikad ei kehti administraatoritele. Microsoft jõustab mis tahes Azure'i administraatorirolli jaoks tugeva kahe väravaga parooli lähtestamise poliitika. Veenduge, et testite kasutajat, kes pole administraator. Administraatori lähtestamispoliitika kohta leiate lisateavet artiklist Administraatori [lähtestamispoliitika erinevused.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Ma ei soovi, et kasutajad registreeriks parooli lähtestamiseks täiendavat turbeteavet**

Saate kasutajate andmeid (meili- ja telefoniatribuute) api, PowerShelli või Azure AD-Ühendus. Lugege, kuidas lugeda.

- [Parooli lähtestamise juurutamine ilma kasutajaid registreerimata](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Milliseid andmeid parooli lähtestamine kasutab?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Soovin, et kasutajad registreeriks parooli lähtestamiseks oma täiendava turbeteabe**

1. Kui soovite, et teie kasutajad registreerivad oma turbeteabe iseteeninduse parooli lähtestamiseks, suunates nad [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Kui kasutaja (kasutaja või administraator) andmed on asustatud, [](https://passwordreset.microsoftonline.com/) suunake kasutaja aka.ms/sspr, et kasutajad saaksid oma paroolid lähtestada.
1. Kui kasutajatel esineb endiselt probleeme, on nad tõenäoliselt ühendatud **või** **parooliga sünkroonitud** kasutajad. See tähendab, et paroolkirjutusteenusega on tõenäoliselt probleeme.