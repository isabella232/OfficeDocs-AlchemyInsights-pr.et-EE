---
title: Teamsi halduskeskus
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
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049340"
---
# <a name="teams-admin-center"></a>Teamsi halduskeskus

Vaadake teavet Teamsi haldamise kohta [Teamsi halduskeskusega](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Kui te ei pääse Teamsi halduskeskusele ligi, kontrollige järgnevat.

- Veenduge, et oleksite lubanud õige [Office 365 IP-aadressid ja URL-id](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) kõikidel perimeetriseadmetel (tulemüür jne) või tulemüüri reeglid teie kohalikus masinas.
- Veenduge, et Teamsi halduskeskuse portaali juurdepääsuks kasutatav sisselogimisteave ühtiks [Microsoft 365 haldusportaalis](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) loetletud kasutajanimega.

Kui kasutajad ei ilmu Teamsi halduskeskuses, kontrollige järgnevat.

- Kas olete kasutajad loonud või määranud itsentsid viimase 24 tunni jooksul? Veenduge, et ootaksite vähemalt 24 tundi enne tugiteenusetaotluse avamist.
- Veenduge, kas olete määranud sobivad litsentsid.
- Kui teil on kohapealne Active Directory, veenduge, et kohaliku Active Directory väljal [ProxyAddresses oleva msRTCSIP-PrimaryUserAddressi](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) või SIP-aadressi väärtus on kordumatu ja vorming vastab **sip:** kasutaja kasutajanimi [Microsoft 365 halduskeskus](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Kui kavatsete säilitada Skype'i ärirakenduse server juurutuse ning kasutajad on kodus kohapeal ja võrgus: järgige oma Skype'i ärirakenduse server juhtpaneelil linki **"Teams** ja Skype'i ärirakendus Online'iga hübriidjuurutus" ja teisaldage kasutajad võrgus.
