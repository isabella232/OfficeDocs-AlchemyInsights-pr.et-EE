---
title: Teatised Yammeris
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
- "9002878"
- "5480"
ms.openlocfilehash: 8e7c03f2b557a7d3c409b2ee418df055d0569ee6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833575"
---
# <a name="notifications-in-yammer"></a>Teatised Yammeris

Asjakohastes vestlustes uuest tegevusest teavitamiseks [saadab Yammer teavitusi](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) kas meili teel või kui kasutate Yammerit mobiilsideseadmes, siis läbi tõuketeatiste. Vaikimisi saadab Yammer teatisi paljude tegevusetüüpide kohta teie võrgus. Kasutajad saavad värskendada oma meilisõnumite sätteid läbi Yammeri veebisaidi ja tõuketeatisi konfigureeritakse mobiilirakenduse kaudu. 

Yammer on lisanud [Outlooki interaktiivset meilisõnumite](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420) spikri. Osad meilisõnumid (sõnumi koopia) muutub Outlooki veebirakenduses interaktiivseks. Tulevane värskendus toob selle Outlooki teistesse versioonidesse.

**Yammeri teatiste tüübid**

- Meilisõnumid (rühma värskendused, keegi kutsub teid rühma, teile saadetakse sisendkausta sõnum jne).
- Tõuketeatised (saadetakse mobiilsideseadmesse, kui teid mainitakse, sisendkausta saabub sõnum jne).
- Töölaua hüpikaknad (kui teil on installitud Yammeri töölauarakendus, kuvab see teile hüpikteatiseid).
- Kellaga teatised (Yammeri veebisaidil näevad erinevate sündmuste teatiseid. Meiliaadress ega tõuketeatis ei pruugi nende sõnumitega alati seotud olla.)

Saadaval on rohkem [üksikasjalikku teavet teatiste kohta](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Teatiste haldamine**

Kasutajad peavad oma teatisi ise haldama. Saadaval on teave selle kohta, [kuidas Yammeri meilisõnumeid ja mobiiliteatiseid lubada ning keelata](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Administraatorid ei saa kasutajate nimel kõiki teatisi keelata ega juhtida teatisi. Administraatorid saavad [juhtida seda, kas meilisõnumites on lisatud logi ja kas kasutajad peavad kinnitama sõnumeid,](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) mis on postitatud meiliaadressi poolt.

**Teie organisatsioonis paljude kasutajate saadetud meilisõnumite teatised**

Mõnikord saadab Yammer ühe meilisõnumi teatise ja see jõuab organisatsioonis palju rohkemate kasutajateni kui eeldatud. See juhtub, kui Yammerisse lisatakse leviloend või muud tüüpi mitte individuaalne meiliaadress. Yammer ei tea kõikide juhtumite puhu, kas meiliaadress kuulub ühele kasutajale või on tegu meiliaadressiga, mis põhjustab ühe meilisõnumi kohaletoimetamist paljudele saajatele. Selle probleemi esinemisel peate Yammeris [peatama (keelama) selle meiliaadressiga sobimatu kasutaja](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users). 

Selle probleemi esinemise võimaluse vähendamiseks peaksite tegema järgmist.

1. [Jõustama Office 365 identiteedi](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) Yammeri jaoks.
2. Blokeerige välised saajad, et nad ei saadaks teie organisatsioonile meilisõnumeid, või piirake saatjaid kinnitatud loendiga.

Selle probleemi esinemisel tehke järgmist.

1. Tuvastage meilisõnumi saaja, mis peaks ühtima Yammeri kasutajaga. Näiteks all-in-sales@fabrikam.com on kõikide müügiinimeste leviloend. See leviloend on tuvastatav kasutajate saadavate Yammeri meilisõnumite järgi.
2. Kasutage [võrguadministraatoris inaktiveerimise (peatamise) funktsiooni](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users), et peatada meiliaadressiga all-in-sales@fabrikam.com kasutaja. Peatamise võib tagasi võtta, seega on see kustutamisest ohutum. Kasutaja kustutamine leiab 90 päeva pärast automaatselt aset.
3. Teise võimalusena vaadake üle suvand [Kasutaja eksport](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers), et tuvastada teised mitte kasutajate meiliaadressid, mis tuleks peatada.
