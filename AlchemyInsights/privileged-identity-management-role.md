---
title: Priviligeeritud identiteedi haldamise roll
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088676"
---
# <a name="privileged-identity-managementpim-role"></a>Privilegeeritud identiteedi haldamise (PIM) roll

**Pärast rolli aktiveerimist ei anta lube.**

Kui aktiveerite rolli Azure AD priviligeeritud identiteedi halduses (PIM), ei pruugi aktiveerimine kohe levida kõigile portaalidele, mis nõuavad privilegeeritud rolli. Mõnikord, isegi kui muudatus on paljundatud, võib vahemällu salvestamine portaalis põhjustada muudatuse kohese jõustumise.

Kui teie aktiveerimine on hilinenud, tehke järgmist.

1. Logige Azure ' i portaalist välja ja seejärel logige uuesti sisse. Kui aktiveerite Azure AD rolli või Azure ' i ressursi rolli, kuvatakse aktiveerimise etapid. Kui kõik etapid on valmis, kuvatakse link "Logi välja". Selle lingi kaudu saate välja logida. See lahendab enamiku juhtumite aktiveerimise viivitusi.
2. PIM. Veenduge, et olete loetletud rolli liikmena.
3. Kui aktiveerite Exchange ' i administraatori rolli, veenduge, et logite välja ja logite uuesti sisse. Kui probleem ei lahene, avage kasutajatoe pilet ja tõstke see probleemina esile. Kui kasutate turbe-ja vastavuskontrolli keskusele juurdepääsuks Exchange ' i administraatori rolli, lugege järgmist juhist.
4. Kui aktiveerite rolli juurdepääsuks turbele ja nõuetele vastavuse keskusele või kui aktiveerite SharePointi administraatori rolli, kogete mõne minuti jooksul kuni mõne tunni jooksul mõningast aktiveerimise viivitust. See on teadaolev probleem ning me töötame nende meeskondadega aktiivselt selle probleemi lahendamiseks niipea kui võimalik.

Lisateavet leiate järgmisest teemast.

- [Azure AD rollide aktiveerimine PIM-s](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Azure ' i ressursside rollide aktiveerimine PIM-s](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Õiguseid ei eemaldata pärast rolli desaktiveerimist või rolli aktiveerimise lõppemist**

Kui desaktiveerite rolli Azure AD priviligeeritud identiteedi halduses või kui rolli aktiveerimise periood aegub, võib esineda viivitusi, kus teil on jätkuvalt juurdepääs.

Kui teie desaktiveerimine on hilinenud, järgige järgmisi juhiseid.

1. Kui desaktiveerite Exchange ' i administraatori rolli või rolli aktiveerimise periood aegub, ja märkate, et enne õiguste eemaldamist on oluline viivitamine, avage tugiteenuste pakett ja teavitage oma klienditoe tehnikut, et saaksite Office ' i selle probleemi lahendamiseks kasutada privilegeeritud juurdepääsu haldust (PAM).
2. Kui aktiveerimise aeg on aegunud, kuid brauseri seanss on endiselt avatud, sulgege brauser. Kui olete selle seansi sulgenud, saate rolli edasi kasutada. See on teadaolev probleem ja me otsime võimalikku lahendust iga seansi aktiivseks tühistamiseks, kui aktiveerimine on aegunud.

Kui teie viivitus on erinev kui need kaks stsenaariumit, siis avage kasutajatugi.
