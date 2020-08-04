---
title: Intune ' i administraatori konsooli kasutamise probleemid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555037"
---
# <a name="problems-using-the-intune-admin-console"></a>Intune ' i administraatori konsooli kasutamise probleemid

**Intune ' i administraatori portaali navigeerimisel "juurdepääs keelatud".**

- Kui olete kohandatud rolli Intune ' i liige, veenduge, et teie kontole on määratud Intune ' i või Enterprise Mobility Suite (EMS) litsents.
- Kui kasutate seadmete haldamiseks Configuration Manageri, siis veenduge, et te ei kuuluks Configuration Manageri MDM-i kasutaja kollektsiooni Intune ' i.
- Veenduge, et teile on määratud roll-põhine halduse kontrolli (RBAC) load Intune rollid Blade.
- Veenduge, et kasutatav rühm pole leviloend. Azure ' i portaalis saab Intune ' i ainult toetada kasutajakontosid, mis kuuluvad Azure Active Directory turbe rühmadesse. Vaadake üle oma rühmad Azure ' i portaalis > **Intune**' i  >  **rühmad**või Azure ' i portaalis > **Azure Active Directory**.

**Kasutajal on määratud Intune ' i rolli jaoks liiga palju õiguseid**

Soovitage kasutajal minna Intune Intune **Intune**  >  **Rollidele**, mida  >  **minu load**  >  **ekspordivad** antud õigustega tutvumiseks.

**Lisasin rollile rühma ulatuse, kuid selle rolli kasutajad näevad endiselt teisi kasutajaid või seadmeid.**

Rakendusala rühmad ei Filtreeri kasutajaid ega seadmeid. Rakendusala rühmad:

- Saate piirata, kellele kasutajad saavad poliitikaid või rakendusi määrata.
- Lubada ainult kindlatel kasutajatel kasutada seadmeid, mis ei tööta.

Lisateavet ulatuste rühmade kohta leiate artiklist [Role-Based Access Control (RBAC) Microsoft Intune ' is](https://docs.microsoft.com/intune/role-based-access-control).

**Lisasin kasutaja Intune rollile, kuid neil on endiselt täielik juurdepääs Intune konsoolile.**

Liikuge Azure ' i portaalis > **kasutajate** Intune ' i ja veenduge, et kasutaja poleks määratud Azure ' i portaalis ühelegi järgmistest rollidest.

- Globaalne administraator
- Teenuse administraatori Intune
- SharePointi administraator

Lisateavet leiate artiklist [Role-Based Access Control (RBAC) Microsoft Intune ' is](https://docs.microsoft.com/intune/role-based-access-control).

**Accessi probleemid**

Lisateavet leiate teemast [Office 365, Azure ' i või Intune ' i sisselogimine](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).