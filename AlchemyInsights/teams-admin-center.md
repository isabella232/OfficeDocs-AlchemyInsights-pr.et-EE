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
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826375"
---
# <a name="teams-admin-center"></a>Teamsi halduskeskus

Vaadake teavet Teamsi haldamise kohta [Teamsi halduskeskusega](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Kui te ei pääse Teamsi halduskeskusele ligi, kontrollige järgnevat.

- Veenduge, et oleksite lubanud õige [Office 365 IP-aadressid ja URL-id](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) kõikidel perimeetriseadmetel (tulemüür jne) või tulemüüri reeglid teie kohalikus masinas.
- Veenduge, et Teamsi halduskeskuse portaali juurdepääsuks kasutatav sisselogimisteave ühtiks [Microsoft 365 haldusportaalis](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) loetletud kasutajanimega.

Kui kasutajad ei ilmu Teamsi halduskeskuses, kontrollige järgnevat.

- Kas olete kasutajad loonud või määranud itsentsid viimase 24 tunni jooksul? Veenduge, et ootaksite vähemalt 24 tundi enne tugiteenusetaotluse avamist.
- Veenduge, kas olete määranud sobivad litsentsid.
- Kui teil on kohapealne Active Directory, veenduge, et kohaliku Active Directory väljal [ProxyAddresses oleva msRTCSIP-PrimaryUserAddressi](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) või SIP-aadressi väärtus on kordumatu ja vorming vastab **sip:** Kasutaja kasutajanimi [Microsoft 365 halduskeskusest](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Kui kavatsete säilitada Skype'i ärirakenduse serveri juurutuse ning kasutajad on kodus kohapeal ja veebis, järgige Skype'i ärirakenduse serveri juhtpaneelil linki "Hübriidrakenduse loomine Teamsi ja Skype'i ärirakenduse **veebiväljaandega"** ja teisaldage kasutajad veebiväljaandes.
