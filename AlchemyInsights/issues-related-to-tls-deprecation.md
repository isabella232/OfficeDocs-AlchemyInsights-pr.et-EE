---
title: Ei saa saata/vastu võtta meilisõnumeid teenusest Office 365 TLS 1,0 ja TLS 1,1 keelamise tõttu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743969"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Ei saa saata/vastu võtta meilisõnumeid teenusest Office 365 TLS 1,0 ja TLS 1,1 keelamise tõttu

Nagu kinnitas sõnumikeskuse postituse MC229914, TLS 1,0 ja TLS 1,1, hakkas jõustamine Exchange Online ' i meilivoo lõpp-punktide korral. Varsti Office 365 ei nõustu enam TLS 1,0 ja TLS 1,1 väliste allikate kaudu. Samuti ei kasuta Exchange Online kunagi TLS 1,0 või 1,1 Väljamineva meili saatmiseks. Kui teil on probleeme TLS 1,0 või 1,1 keelamise tõttu, võib ilmneda üks järgmistest tõrketeadetest.

- Saatja saab NDR-i tagasipõrkamise tagasi-' 421 4.4.2 Connection langes tõttu SocketError '
- Tõrge asutusesisese serveri järjekorra vaaturis, mis saadab meilisõnumeid ametnikule 365-' 421 4.4.2 Connection langes SocketError tõttu
- Tõrge rakenduses saada konnektor [protokolli logimine](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) serveris, mis saadab meilisõnumid Office 365-TLS-i läbirääkimistele nurjus tõrkega SocketError
- Viga saatmisel või vastuvõtmisel konnektori protokolli log-"451 5.7.3 peab esmalt välja andma STARTTLS käsu"

Kui teil ilmneb mõni eespool kirjeldatud tõrgetest, veenduge, et meili saatmiseks või vastuvõtmiseks loodud serveris on TLS 1,2 lubatud, kontrollides järgmisi registrivõtmed.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ klient] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ Server] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**

Kui muudate ülaltoodud registrivõtmed, et lubada TLS 1,2, taaskäivitage server muudatuste jõustumiseks. Veenduge ka, et teil oleks installitud uusimad Windowsi ja Exchange ' i värskendused.

Lisateavet leiate järgmistest teemadest:

- [Exchange Serveri TLS-i juhised, osa 1: TLS 1,2-i ettevalmistamine – Microsoft Techi kogukond](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Serveri TLS-i juhised osa 2: TLS 1,2 lubamine ja klientide tuvastamine, kes seda ei kasuta-Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [E-posti stsenaariumite mõistmine, kui TLS-versioone ei saa Exchange Online ' iga kokku leppida – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
