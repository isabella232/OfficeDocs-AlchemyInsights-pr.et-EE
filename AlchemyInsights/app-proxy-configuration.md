---
title: Rakenduse puhverserveri konfigureerimine
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885137"
---
# <a name="app-proxy-configuration"></a>Rakenduse puhverserveri konfigureerimine

1. Kui soovite teada saada, kuidas konfigureerida rakenduse puhverserveri rakendust Azure AD-s asutusesisesete rakenduste pilve jaoks, lugege teemat [rakenduse puhverserveri rakenduse konfigureerimine](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Ühekordne sisselogimine (SSO) võimaldab kasutajatel kasutada rakendust, autentimata mitu korda. See lubab ühes autentimisel esineda pilves, Azure Active Directory vastu ning lubab teenusel või konnektori kasutajal jäljendada kasutajat, kes täidavad rakenduse jaoks täiendavaid autentimise probleeme. Lisateavet leiate teemast [ühekordse sisselogimise konfigureerimine rakenduse puhverserveri rakendusse](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Kasutage [seda artiklit](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) levinud probleemide tõrkeotsinguks, kui loote uue rakenduse puhverserveri rakenduse.
4. Kui teil on probleeme rakenduse back-end autentimise häälestamisega, peate võib-olla lahendama [Kerberose piiratud delegeerimise konfiguratsioonid rakenduse puhverserveri jaoks](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) või järgima juhiseid [rakenduse konfigureerimise kohta PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) abil probleemi lahendamiseks.
