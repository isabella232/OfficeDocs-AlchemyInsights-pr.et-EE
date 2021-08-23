---
title: Kas soovite Microsoftile teatada valepositiivsest rämpspostist?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396611"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Kas korralikud meilisõnumid märgitakse rämpspostiks?

See on masendav, kui seaduslik meilisõnum on rämpspostikaustas või karantiinis. Kaaluge järgmisi valepositiivsete põhjuste kõige levinumaid põhjuseid.

**Rentniku alistamine (kõige levinum)** See on täielikult teie kontrolli all, et parandusi teha.

Edastage sõnum Microsoft 365 Defender poliitikate ja reeglite analüüsimiseks; uuesti skannimise üksikasjad on saadaval mõne minuti jooksul.
Vaadake poliitikad või reeglid läbi või muutke neid vastavalt vajadusele. 

**Lõppkasutaja alistab (levinud)** See on täielikult teie kontrolli all, et parandusi teha. 

Edastage sõnum Microsoft 365 Defender poliitikate ja reeglite analüüsimiseks; uuesti skannimise üksikasjad on saadaval mõne minuti jooksul. 

Kui sõnum blokeeriti, kuna see saadeti kasutaja blokeeritud saatjate loendis aadressilt, sisaldavad päised rämpsposti filtreerimise verdikti "SFV:BLK".

**Saatjate meiliautentimine** See on osaliselt teie kontrolli all, et parandusi teha.

Saatke sõnum, et analüüsida kohaletoimetamise ajal saatja meiliautentimise tõrkeid; tulemused on saadaval päeva jooksul. 

Kui teil on saatmistaristu, vaadake üle, kuidas seda koos SPF-, DKIM- ja DMARC-ga joondada, veendumaks, et sihtmeilisüsteemid usaldavad teie domeenist saadetud sõnumeid. Teise võimalusena võtke saatjatega ühendust, et tegeleda oma DNS-i konfiguratsioonidega.

**Microsofti filtreerimise otsused** See on osaliselt teie kontrolli all, et parandusi teha.

Saatke sõnum ja teatage sõnumist turvaliselt; tulemuste uuesti skannimine on saadaval päeva jooksul. Kasutage rentniku lubamis-/blokeerimisloendit, kui te ei nõustu teatud olukordades otsuse filtreerimisega. Siiski ei tohiks te jäädavalt Microsofti filtreerimistest mööduda. 

Lisateavet leiate järgmistest teemadest.

- Saate lubada lõppkasutajatel sõnumeid Microsoftile edastada. Microsoft kasutab neid edastusi meilikaitsetehnoloogiate tõhususe suurendamiseks ja need kuvatakse edastusaruannetes, mille abil saate poliitikaid värskendada. 

- Lühivideot analüüsimiseks sõnumite edastamise kohta leiate teemast [Sõnumite edastamine analüüsiks.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Administraatorite esitamine microsoftile rämpsposti, andmepüügi, URL-ide ja failide edastamiseks](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Rentniku lubamis-/blokeerimisloendi haldamine](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Rämpspostitõrje sõnumipäised Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Väljamineva rämpsposti kaitse EOP-s](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)