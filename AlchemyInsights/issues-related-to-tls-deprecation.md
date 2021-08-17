---
title: TLS 1.0 ja TLS 1.1 keelamise tõttu ei saa TLS 1.0 ja TLS 1.1 Office 365-le meilisõnumeid saata/vastu võtta
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054902"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>TLS 1.0 ja TLS 1.1 keelamise tõttu ei saa TLS 1.0 ja TLS 1.1 Office 365-le meilisõnumeid saata/vastu võtta

Nagu kinnitab teatekeskus pärast MC229914, hakkas TLS 1.0 ja TLS 1.1 deprecation Exchange Online meilivoo lõpp-punktide jaoks. Peagi Office 365 ei aktsepteeri TLS 1.0 ja TLS 1.1 meiliühendusi välisallikatest. Samuti Exchange Online TLS 1.0 või 1.1 kasutada väljamineva meili saatmiseks. Kui teil esineb TLS 1.0 või 1.1 keelamise tõttu probleeme, võib ilmneda üks järgmistest tõrgetest.

- Saatja saab NDR-i tagasi- '421 4.4.2 Connection dropped due due SocketError' ("421 4.4.2 Connection dropped due due SocketError" (421 4.4.2 Connection dropped due to SocketError) ("421 4.4.2 Connection dropped due to Socket
- Tõrge asutusesisese serveri järjekorravaaturis, mis saadab meilisõnumeid 365- '421 4.4.2 Connection dropped due due SocketError' (421 4.4.2 Connection dropped due to SocketError)
- Tõrge meili [saatva](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) serveri konnektorprotokolli logis Office 365- TLS-i läbirääkimine nurjus tõrkega SocketError
- Tõrge konnektoriprotokolli logi saatmisel või vastuvõtul – '451 5.7.3 Esmalt tuleb väljastada käsk STARTTLS"

Kui teil esineb mõni ülaltoodud tõrketeade, veenduge, et meili saatva või vastuvõtva serveri jaoks oleks lubatud TLS 1.2, kontrollides järgmisi registrivõtmeid.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Kui muudate TLS 1.2 lubamiseks ülaltoodud registrivõtmeid, taaskäivitage muudatuste jõustumiseks server. Samuti veenduge, et teil oleks installitud uusimad Windows ja Exchange värskendused.

Lisateavet leiate järgmistest teemadest.

- [Exchange Server TLS-i juhised, 1. osa: TLS 1.2 jaoks valmistumine – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS-i juhised 2. osa: TLS 1.2 lubamine ja seda mitte kasutava kliendi tuvastamine – Microsoft Techi kogukond](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Meilistsenaariumide mõistmine, kui TLS-i versioonidega ei saa Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
