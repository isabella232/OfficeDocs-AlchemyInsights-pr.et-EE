---
title: Linkide ja URL-ide probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974303"
---
# <a name="issues-with-links-and-urls"></a>Linkide ja URL-ide probleemid

Suuna URI/vasta URL-id (mõlemad avaldised on omavahel asendatavad) on URL-id, mida kasutab Microsoft Identity Platform, et tagastada rakenduse taotletud märgid. Lisateavet nende URL-ide kohta leiate järgmistest artiklitest.

- [Autentimise vood ja rakenduse stsenaariumid](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – teave ümbersuunamise URI kohta **rakenduse registreerimise** lehel iga stsenaariumi korral.
- [URI/vasta URL-ide ja piirangute ümbersuunamine](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ma ei tea, kuidas registreerida õige ümbersuunamise URI/vastuse URL minu rakenduse jaoks**

Kui logite sisse rakendusega, mida arendate, kui sisselogimise dialoogiboks kuvab **AADSTS50011: taotluses määratud vastuse URL ei vasta rakenduse <your app ID> jaoks konfigureeritud vastamise** URL-idele, peate lisama oma rakenduse registrisse, ümbersuunamise URI, mida kasutati Microsofti identiteedi platvormile sümboolne taotlus.

Vastuse URL-i lisamiseks avage Azure ' i portaalis **rakenduse registreerimise** lehe vahekaart **autentimine** ja lisage kirje jaotise **ümbersuunamine URI** . URI ümbersuunamine on tipitud (veeb või mobiil/töölaud). Sisestatav väärtus sõltub sellest, millist tüüpi rakendust te ehitate, nagu on kirjeldatud allpool.

- Ühe lehe rakenduste ja veebirakenduste jaoks on vastuse URL teie rakenduse URL. Lisateavet leiate teemast [ühe lehekülje registreerimine](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) või [veebirakenduse rakenduse registreerimine Azure ' i portaali kaudu](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Töölaua rakenduste jaoks sõltub väärtus, mida peate valima.
    - platvorm (MacOS erineb Windowsi või Linuxi hulgast)
    - viis, kuidas te omandate tõendi (interaktiivselt, koos seadme koodi voo, Windowsi integreeritud autentimisega [IWA] või kasutajanime/parooliga).
    Lisateavet leiate teemast [töölaua rakendused – rakenduse registreerimine – ümbersuunamise URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobiilsete rakenduste korral sõltub ümbersuunamise URI järgmistest teemadest:
    - platvorm (iOS/Android/UWP)
    - teave, mida kasutatakse rakenduse koostamiseks (nt iOS-i komplekt-ID), ja Androidi Azure ' i portaali rakenduse registreerimise paketi nimi ja allkiri räsi. Lisateavet leiate teemast [platvormi konfigureerimine ja ümbersuunamine URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Veebirakendusliidesed ja mõned märkide hankimiseks ette nähtud vaikivad viisid (IWA ja username/Password) ei nõua ümbersuunamise URI-d.

**Olen juurutanud oma veebirakenduse ja kui katsetan juurutatud rakendust, saan vastuse URL-i mittevastavuse sõnumile**

Lisage ümbersuunamise URI kõigi asukohtade jaoks, kus soovite oma veebirakendust kasutada. Lisateavet leiate teemast [veebirakenduse rakenduse registreerimine Azure ' i portaali kaudu](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Lisa ümbersuunamise URI kohale kohe pärast seda, kui olete rakenduse juurutanud selles asukohas.

**Ma ei saa registreerida piisavalt vastatud URL-e**

Sa oled ISV ja sul on üks või mitu ümbersuunamise URI iga sinu kliendi jaoks. Soovite migreerida ADAL/Azure AD v 1.0 MSAL/Microsoft Identity platvormile ja vajutate [maksimaalset arvu ümbersuunamise URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Selle probleemi lahendamiseks lisage igale kliendile vastavale [teenusele ümbersuunamise URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) .
