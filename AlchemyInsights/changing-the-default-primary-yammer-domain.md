---
title: Yammeri vaikedomeeni muutmine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991132"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Yammeri vaikimi/peamise domeeni muutmine

Yammeri URL sisaldab teie Yammeri võrgu praegust peamist domeeninime. See domeeninimi ei tohi ühtida Office 365-s või Azure AD-s määratud peamise domeeninimega. Rentnikule lisatud kohandatud domeenide arvu põhjal esineb käitumises erinevusi ja selle põhjal, kas Yammer on toetatud konfiguratsioonis (1 rentnik: 1 võrk või 1:1). Saadaval on [Yammeri domeenide ja Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) dokumentatsioon.

Vale domeeni kuvamise kõige levinum põhjus on see, et olemas on mitu Yammeri võrku ja need tuleb konsolideerida. [Üheks võrguks konsolideerimine](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) võrgu migreerimise tööriista kasutades on oluline esimene samm. Tehke seda enne esmase domeeni määramise proovimist.

**Kohandatud domeenid puuduvad**

Uute rentnike jaoks kasutatakse Yammeri jaoks rentniku vaikedomeeni (nt fabrikam.onmicrosoft.com). Peamiseks domeeniks on määratud yammer.com/fabrikam.onmicrosoft.com.

**Üks kohandatud domeen**

Yammer valib automaatselt Yammeri peamiseks domeeniks rentniku kohandatud domeeni (nt fabrikam.com). Selleks määratakse yammer.com/fabrikam.com. Selle muudatuse teeb domeeni sünkroonimisteenus ja selleks jõustumiseks võib kuluda kuni 24 tundi.

**Mitu kohandatud domeeni**

Yammeril saab olla peamine domeen, mis erineb rentniku vaikedomeenist. Kuna kohandatud domeene on mitu, ei proovi Yammer arvata, milline saadaolevatest on õige domeen. Peate avama tugiteenuse juhtumi, et taotleda, et peamine domeeninimi muudetaks teie valitud peamiseks domeeniks.

**Täiendav tõrkeotsingu teave**

Mõnel juhul võivad domeenid olla rentnike vahel liikunud ja domeeni sünkroonimisteenus ei saanud korralikult töötada. Lisaks valele peamisele domeenile võivad teil tekkida sisselogimise ja muud probleemid. Selle probleemi lahendamiseks võib olla vajalik Microsofti tugiteenuste abiga domeenide liigutamine õigesse võrgustikku. See olukord vajab otsest abistamist ja selle lahendamiseks võib kuluda veidi aega, eriti kui domeeninimede loend on väga pikk. Avage seda tüüpi probleemide lahendamisl abi saamiseks tugiteenuse juhtum.

Tugiagendiga töötades nad kontrollivad, kas teie kontrolli all oleva rentniku domeenid on kinnitatud. Nad võivad küsida täiendavaid kontrollküsimusi teie domeenide kohta, kui need on teie rentnikule lisatud, kuid pole DNS-i poolt kinnitatud. Veenduge, et domeenid oleksid DNS-i poolt kinnitatud, et kiirendada protsessi.
