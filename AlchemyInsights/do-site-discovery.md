---
title: Saidi tuvastamine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692935"
---
# <a name="do-site-discovery"></a>Saidi tuvastamine

Kui teie ettevõte kasutab endiselt pärandist veebirakendusi ja plaanib kasutada Internet Exploreri režiimi (mida enamik kliente ei kasuta), peaksite tegema mõne muu saidi tuvastamise.

**Olete juba juurutanud Microsoft Edge ' i varasema versiooni**

Kui olete oma ettevõtte saidi loendi juba konfigureerinud töötama Microsoft Edge ' i Legacy-versioonis, on teie saidi tuvastus peaaegu valmis. Võimalik, et peate lisama neutraalseid saite.

Neutraalsed saidid on tavaliselt saidid, mis pakuvad ühekordse sisselogimise (SSO). Kui lähete Microsoft Edge ' i neutraalsele saidile, soovite autentida Microsoft Edge ' i. Kui lähete Internet Exploreri režiimis neutraalsele saidile, siis soovite autentida Internet Exploreri režiimis.

Tuvastage kõik SSO või muud neutraalsed saidid, mida kasutate, ja lisage need oma ettevõtte saidi loendisse.

**Internet Explorer on teie vaikebrauser**

Kui kasutate praegu ainult Internet Explorerit, ei pruugi te teada saada, millised saidid on täiendatud moodsate veebistandarditega ja mis vajavad endiselt Internet Explorerit. Te soovite leida ja lisada need saidid ettevõtte saidi loendisse, et saaksite kasutada Internet Exploreri režiimi ainult nende saitide jaoks.

> [!NOTE]
> [Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) avastab saidid, mis võivad vajada Internet Exploreri režiimi. See võib koguda andmeid arvutites, kus töötab Windows Internet Explorer 8 Internet Explorer 11 kaudu opsüsteemis Windows 10, Windows 8,1 või Windows 7.

**Andmete analüüsimine**

Kui olete saidi andmed kogunud, soovitame andmete analüüsimiseks järgmisi nelja-etapilisi toiminguid.
1. Sortige andmed domeeni järgi ja seejärel URL-i järgi.
2. Saate määratleda Internet Exploreri režiimi konfigureerimiseks kasutatava rakenduse piirid. Soovite kaasata kõik rakenduse määratlevad saidid ja veebihaldused, kuid te ei soovi lisada täiendavaid saite ja juhtelemente. Mõned saidid võivad olla nii lihtsad, kui *https://contoso.com/app1* teised võivad nõuda mitme saidi ja lehe määratlemist.
3. Testige rakendust, et veenduda, et see ei tööta algupäraselt. Paljud saidid pakuvad moodsat brauserit, kui nad avastavad modernse brauseri ja pakuvad Internet Exploreri tuvastamisel ainult pärandist sisu.
4. Lisage rakendus oma ettevõtte saidi loendisse, kui test nurjub.

> [!NOTE]
> Parima tavana rühmitage kõik saidid, mis moodustavad rakenduse. Nii on rakenduse täiendamisel hõlpsam eemaldada kogu sait Internet Exploreri režiimist ja alustada selle rakenduse jaoks moodsate brauserite kasutamist.

Kui olete saidi tuvastamisega lõpetanud ja olete andmed analüüsinud, olete valmis alustama oma kanali strateegiat.

