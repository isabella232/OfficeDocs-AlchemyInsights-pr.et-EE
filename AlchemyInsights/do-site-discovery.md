---
title: Saidituvastuse leidmine
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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030754"
---
# <a name="do-site-discovery"></a>Saidituvastuse leidmine

Kui teie ettevõte kasutab endiselt pärandveebirakendusi ja -plaane Internet Exploreri režiimi (mida enamik kliente teeb), peaksite tegema täiendavaid saidituvastusi.

**Olete juba juurutanud vanema versiooni Microsoft Edge**

Kui olete ettevõttesaidiloendi juba konfigureerinud töötama Microsoft Edge versiooni jaoks. Võimalik, et peate lisama neutraalsed saidid.

Neutraalsed saidid on tavaliselt saidid, mis pakuvad ühekordset sisselogimist (SSO). Kui lähete neutraalsele saidile Microsoft Edge, siis soovite jääda Microsoft Edge autentimiseks. Kui lähete Internet Exploreri režiimis neutraalsele saidile, siis soovite autentimiseks internet Exploreri režiimis püsida.

Tuvastage kõik SSO-d või muud neutraalsed saidid, mida kasutate, ja lisage need ettevõttesaitide loendisse.

**Internet Explorer on teie vaikebrauser**

Kui kasutate praegu ainult Internet Explorerit, ei pruugi te teada, millised saidid on nüüd kasutusele võtnud tänapäevased veebistandardid ja mis nõuavad endiselt Internet Explorerit. Soovite need saidid ettevõttesaitide loendisse üles leida ja lisada, et internet Exploreri režiimi saaks kasutada ainult nende saitide jaoks.

> [!NOTE]
> [Ettevõttesaidi tuvastuse](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) abil tuvastatakse saidid, mis võivad vajada Internet Exploreri režiimi. See võib koguda andmeid arvutites, kus töötab Windows Internet Explorer 8 internet Explorer 11 Windows 10, Windows 8.1 või Windows 7.

**Andmete analüüsimine**

Pärast saidiandmete kogumist soovitame andmete analüüsimiseks teha järgmist neljaastmelise protsessi.
1. Sortige andmed domeeni järgi ja seejärel URL-i järgi.
2. Määratlege Rakenduse piirid Internet Exploreri režiimi jaoks konfigureerimiseks. Soovite kaasata kõik saidid ja veebi juhtelemendid, mis rakenduse määratlevad, kuid te ei soovi lisada täiendavaid saite ega juhtelemente. Mõned saidid võivad olla sama lihtsad, *https://contoso.com/app1* kui teised võivad nõuda mitme saidi ja lehe määratlemist.
3. Testige rakendust veendumaks, et see ei tööta oma emakeelena. Paljud saidid pakuvad modernse sisuga sisu, kui nad tuvastavad tänapäevase brauseri ja pakuvad pärandsisu ainult Internet Exploreri tuvastamisel.
4. Lisage rakendus ettevõttesaidi loendisse, kui see testimine nurjub.

> [!NOTE]
> Parima tavana saate rühmitada kõik saidid, mis sisaldavad rakendust. Nii on rakenduse versioonitäienduse korral hõlpsam eemaldada kogu sait Internet Exploreri režiimist ja hakata kasutama selle rakenduse jaoks kaasaegset brauserit.

Kui olete saidituvastuse lõpetanud ja olete andmed analüüsinud, saate hakata oma kanalistrateegiat otsima.

