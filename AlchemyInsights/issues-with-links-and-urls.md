---
title: Linkide ja URL-idega seotud probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321903"
---
# <a name="issues-with-links-and-urls"></a>Linkide ja URL-idega seotud probleemid

Ümbersuunamise URI/vastuse URL-id (mõlemad avaldised on asendatavad) on URL-id, mida Microsofti identimisplatvorm kasutab rakenduste taotletud sõnede tagastamiseks. Lisateavet nende URL-ide kohta leiate järgmistest artiklitest:

- [Autentimisvood ja rakenduse stsenaariumid](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - teave URI-ide ümbersuunamise kohta lehel **Rakenduse registreerimine** iga stsenaariumi jaoks.
- [Ümbersuunamise URI/vastuse URL-i kitsendused ja piirangud](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ma ei tea, kuidas registreerida rakenduse jaoks õige ümbersuunamise URI või vastuse URL**

Kui logite sisse koos arendatava rakendusega ja sisselogimisdialoogis kuvatakse **AADSTS50011: taotluses määratud vastuse URL ei vasta rakenduse jaoks konfigureeritud vastuse URL-idele <your app ID>**, peate oma rakenduse registreerimisele lisama ümbersuunamise URI, mida teie kood kasutas sõne taotluses Microsofti identiteediplatvormile.

Vastuse URL-i lisamiseks minge oma lehel **rakenduse registreerimine** Azure'i portaali vahekaardile **Autentimine** ja lisage kirje jaotises **URI-de ümbersuunamine**. Sisestatav väärtus sõltub loodava rakenduse tüübist, nagu allpool on kirjeldatud:

- Ühe lehega rakenduste ja veebirakenduste puhul on vastuse URL teie rakenduse URL. Vaadake [Ühelehelise rakenduse registreerimine](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) või [Veebirakenduse registreerimine Azure'i portaalis](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Töölauarakenduste puhul sõltub valitav väärtus järgnevast:
    - platvormist (MacOS erineb Windowsist või Linuxist)
    - viisist, kuidas te loa hankisite (interaktiivselt, seadme koodivooga, integreeritud Windowsi autentimisteenusega (IWA) või kasutajanime/parooliga).
    Üksikasjad leiate teemast [Töölauarakendused - rakenduse registreerimine - URi ümbersuunamine](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobiilsideseade rakenduste ümbersuunamise URI sõltub järgnevast:
    - platvormist (iOS/Android/UWP)
    - rakenduse loomiseks kasutatud teavest (nt komplekti ID iOS-is ning paketi nimi ja allkirja räsiväärtus Androidis). Azure'i portaali rakenduse registreerimine aitab teid. Lisateavet leiate teemast [Platvormi konfigureerimise ja ümbersuunamise URI-d](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

**Märkus.** Veebi API-d ja mõned märkide (IWA ja kasutajanime/parooli) hankimise vaiksed viisid ei nõua ümbersuunamise URI-d.

**Juurutasin oma veebirakenduse ja juurutatud rakenduse testimisel saan vastuseks URL-i lahknevuse teate**

Lisage ümbersuunamise URI-d kõigi nende asukohtade jaoks, kus te oma veebirakendust juurutate. Lisateavet leiate teemast [Registreerige veebirakendused kasutades Azure‘i portaali](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

**Märkus.** Lisage asukoha ümbersuunamise URI kohe pärast seda, kui olete rakenduse selles asukohas juurutanud.

**Ma ei saa registreerida piisavalt vastuse URL-e**

Olete sõltumatu tarkvaratootja (ISV) ja teil on igale kliendile üks või mitu ümbersuunamise URI. Soovite versioonist ADAL/Azure AD v1.0 migreerida MSAL/Microsofti identimisplatvormile ning te olete jõudnud [maksimaalse ümbersuunamise URI-de arvuni](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Probleemi lahendamiseks [lisage ümbersuunamise URI-d teenusesubjektitele](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) mis vastavad igale teie kliendile.
