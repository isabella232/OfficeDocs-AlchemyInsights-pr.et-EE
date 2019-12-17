---
title: Otsi SharePoint Online ' is
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044039"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Sisu analüüsimine ja indekseerimine SharePoint Online

Sisu tuleb analüüsida ja lisada kasutajate otsinguregistrisse, et leida, mida nad otsivad SharePoint Online ' is. Sisu indekseerida automaatselt eelnevalt määratletud analüüsigraafiku alusel (analüüsigraafikut ei saa muuta). Ämblik valib sisu, mis on muutunud pärast viimast analüüsi ja uuendab indeksit. Et tagada sisu analüüsimine ja indeks värskendatakse, arvestage järgmist.

- Veenduge, et sisu saab otsida, [muutes saidi sisu otsitavaks](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Kui olete muutnud Hallatava atribuudi või kui olete muutnud analüüsitud ja hallatavate atribuutide vastendust, tuleb sait enne muudatuste kajastamist otsinguregistris uuesti indekseerida. 

    Kuna muudatused tehakse otsinguskeemis ja mitte tegeliku saidiga, ei Indekseeri ämblik saiti automaatselt ümber. 

    Lisateabe saamiseks vaadake [käsitsi päringu analüüsimine ja uuesti indekseerimine saidi, teegi või loendi](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Oodake vähemalt 24 tundi pärast käsitsi analüüsi ja täielik uuesti indeks, et näha, kas teil on endiselt probleeme. 

    Kui pärast analüüsi algatamist ja täielikku uuesti indeksit on möödunud rohkem kui 24 tundi, logige palun tugiteenuse Teenindusjuhtumit. Paljudel juhtudel oleme juba lahenduse kallal töötanud. Palun andke meile vähemalt 24 tundi, et lahendus lõpule viia.

> [!IMPORTANT]
> Kui sait, dokument (teek) või loend on kustutatud ja endiselt kuvatakse otsingutulemustes, kasutajad peaksid saama **tõrketeate 404 faili ei leitud** , kui proovite sellele juurde pääseda. See probleem tuleks sisse logitud tugiteenuse juhtumi edasiseks uurimiseks. 



