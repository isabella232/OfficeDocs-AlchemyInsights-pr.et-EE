---
title: Tõrkeotsing Juurdepääs keelatud sõnumitele OneDrive for Business saitidele
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957789"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Tõrkeotsing Juurdepääs keelatud sõnumitele OneDrive for Business saitidele

See probleem ilmneb kõige sagedamini siis, kui kasutaja kustutatakse ja luuakse uuesti sama kasutajasubjektinimega (UPN). Uue konto loomiseks kasutatakse erinevat PUID-i (Passport Unique ID) väärtust. Kui kasutaja proovib juurde pääseda saidikogumile või tema OneDrive, on kasutajal vale PUID. Teine stsenaarium hõlmab kataloogisünkroonimist Active Directory organisatsiooniüksusega (OU). Kui kasutajad on juba SharePoint sisse loginud ja seejärel teisaldatakse teise OU-sse ja sünkroonitakse SharePoint, võib see probleem ilmneda.

1. Selle probleemi lahendamiseks peaksite algse UPN-i taastama artiklis toodud juhiste järgi, [taastage kasutaja](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)Microsoft 365 .
2. Kui te ei saa algset kasutajat taastada, peaksite vana kasutaja OneDrive eemaldama, kasutades neid juhiseid, [eemaldage kasutaja kasutajateabe loendist.]() 
3. Kui see on tehtud, saate kinnitada, et kasutajal on OneDrive administraatoriõigused, järgides juhiseid, mis on toodud jaotises Administraatorite lisamine [kasutaja OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Õigusetasemete kohta leiate lisateavet artiklist Õigusetasemete mõistmine [SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
