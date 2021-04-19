---
title: Yammeri vaikedomeeni muutmine
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
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817952"
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
