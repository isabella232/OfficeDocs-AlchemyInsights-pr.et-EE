---
title: Parooli logid
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
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525136"
---
# <a name="password-logs"></a>Parooli logid

**Mul on probleeme parooli lähtestamise auditilogi logidele juurdepääsuga**

Parooli lähtestamise auditi logidele juurdepääsuga seotud probleemide tõrkeotsingu sooritamiseks tehke järgmist.

Veenduge, et teil on õigus vaadata auditi logisid. 

Lubatud on ainult järgmised rollid.
 - Globaalne administraator
 - Security Administrator
 - Security Reader

**Soovin näha kõiki parooli lähtestamise auditeid alates hetkest, kui ma algselt juurutasin**

Kuni 120 000 parooli lähtestamise/registreerimise sündmusi talletatakse viimase 30 päeva aruannetes. See piirmäär rakendub CSV-i allalaadimisel UI-le. 1 000 000 sündmused on saadaval PowerShelli kaudu.
Lisateavet leiate järgmistest linkidest.

- [Iseteeninduskeskuse parooli lähtestamise sündmused Azure AD aruannetes ja sündmuste API-s](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Parooli lähtestamise registreerimise sündmuste Kiire allalaadimine PowerShelli abil](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Soovin saada lisateavet salasõna lähtestamise aruandluse võimaluste kohta**

Kontrollige, kes registreerub või lähtestab paroolid Azure AD Password reset auditiga Azure ' i portaalis jaotises **kasutajad ja rühmad**.
Lisateavet leiate järgmistest linkidest.

- [Parooli lähtestamise aruannete ülevaade](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Kuidas vaadata Azure ' i portaalis parooli lähtestamise aruandeid?](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Iseteeninduskeskuse parooli lähtestamise sündmused Azure AD aruannetes ja sündmuste API-s](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Parooli lähtestamise registreerimise sündmuste Kiire allalaadimine PowerShelli abil](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


