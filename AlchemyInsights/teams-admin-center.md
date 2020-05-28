---
title: Teamsi halduskeskus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354084"
---
# <a name="teams-admin-center"></a>Teamsi halduskeskus

Vaadake teavet Teamsi haldamise kohta [Teamsi halduskeskusega](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Kui te ei pääse Teamsi halduskeskusele ligi, kontrollige järgnevat.

- Veenduge, et oleksite lubanud õige [Office 365 IP-aadressid ja URL-id](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) kõikidel perimeetriseadmetel (tulemüür jne) või tulemüüri reeglid teie kohalikus masinas.
- Veenduge, et Teamsi halduskeskuse portaali juurdepääsuks kasutatav sisselogimisteave ühtiks [Microsoft 365 haldusportaalis](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) loetletud kasutajanimega.

Kui kasutajad ei ilmu Teamsi halduskeskuses, kontrollige järgnevat.

- Kas olete kasutajad loonud või määranud itsentsid viimase 24 tunni jooksul? Veenduge, et ootaksite vähemalt 24 tundi enne tugiteenusetaotluse avamist.
- Veenduge, kas olete määranud sobivad litsentsid.
- Kui teil on-premise Active Directory, veenduge, et [msRTCSIP PrimaryUserAddress või SIP-aadress väljale ProxyAddresses kohaliku Active Directory on unikaalne ja vorming vastab](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP: kasutaja [Microsoft 365 administreerimiskeskuse](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**kasutajanimi** .
- Kui kavatsete hoida Skype ' i Business Serveri juurutamine ja on kasutajad homed asutusesisese ja online: järgige **"Seadista hübriid meeskonnad ja Skype Business Online"** Skype ' i Business Server juhtpaneeli ja teisaldage Kasutajad online.
