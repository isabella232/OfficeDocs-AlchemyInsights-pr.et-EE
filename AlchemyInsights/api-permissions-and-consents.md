---
title: API-õigused ja nõusolek
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932093"
---
# <a name="api-permissions-and-consent"></a>API-õigused ja nõusolek

Rakendused, mis Microsofti identimisplatvorm, järgivad autoriseerimismudelit, mis annab kasutajatele ja administraatoritele õiguse andmetele juurde pääseda. Autoriseerimismudeli rakendamist on värskendatud Microsofti identimisplatvorm lõpp-punktis. See muudab seda, kuidas rakendus peab Microsofti identimisplatvorm. [Microsofti identimisplatvorm](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) lõpp-punkti õigused ja nõusolek hõlmab selle autoriseerimismudeli põhimõisteid (sh ulatused, õigused ja nõusolek).

Azure [AD Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) nõusoleku raamistik hõlbustab mitme rentnikuga veebi ja kohalike klientrakenduste välja töötamist. Need rakendused lubavad azure AD rentniku kasutajakontode sisselogimist, mis erineb sellest, kus rakendus on registreeritud. Lisaks teie veebi API-le võib neil olla vaja juurde pääseda veebi API Graph API-le (Azure AD,Intune'ile ja teenustele Microsoft 365-is) ja muudele Microsofti teenused'i API-le.

