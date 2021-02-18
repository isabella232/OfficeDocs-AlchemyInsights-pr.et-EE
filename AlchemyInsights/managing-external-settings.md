---
title: Väliste sätete haldamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294213"
---
# <a name="managing-external-settings"></a>Väliste sätete haldamine

**Teadaanne**

- [Google ' i WebView väljalogimine alates jaanuarist 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support). Kontrollige, kas teie rakendused mõjutavad teie rakendusi, järgides Google ' i juhiseid ühilduvuse testimise kohta.
- Veenduge, et kasutate oma kasutajatele Google ' i kontoga sisselogimisel süsteemi WebView või süsteemi brauserit.

**Kutse sätete haldamine**

Veenduge, et olete [konfigureerinud väliskoostöö sätted](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) , et lubada vastavatel inimestel kutsed saata.

**Külaliste pääsuõiguste haldamine**

1. Globaalsed administraatorid saavad hallata Külastajate juurdepääsu kasutusõigusi Azure ' i portaali kaudu, konfigureerides Guest Access permissions lehel välise koostöö sätted. Lisateavet [selle häälestamise kohta](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).
2. Kui soovite, et külalised pääseksid juurde sellistele rakendustele nagu meeskonnad või SharePointi, kinnitate, et olete konfigureerinud need rakendused lubama juurdepääsu külastajatele. Lugege lisateavet [teamsi sätete](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) ja [SharePointi](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)kohta.

**Kutsete konfigureerimine.**

- [Luba B2B väline koostöö ja Halda, kes saavad külalisi kutsuda](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kindlatelt organisatsioonidelt kasutajate kutsete lubamine või keelamine](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**Lubatud identiteedi pakkujate konfigureerimine.**

- [Google Federation](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Otse Föderatsioon](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Meili ühekordne pääsukoodi autentimine](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
