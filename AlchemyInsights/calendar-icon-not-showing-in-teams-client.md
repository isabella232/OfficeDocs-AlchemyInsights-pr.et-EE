---
title: Kalendri ikooni ei kuvata Teamsi klientrakenduses
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
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819949"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalendri ikooni ei kuvata Teamsi klientrakenduses

Teamsi vahekaart Kalender vajab Exchange’i veebiteenuste kaudu juurdepääsu Exchange’i postkastile. Exchange’i postkast võib olla veebipõhine või kohapealne. Veebiversiooni kasutajate puhul, kes vahekaarti Kalender ei näe, veenduge, et neil [oleks Exchange Online’i postkasti litsents ja postkast oleks lubatud](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Kui kasutajal on Exchange Online’is kehtiv postkast, kuid nad endiselt vahekaarti Kalender ei näe, võib teil olla probleem võrguga. Kasutage [Microsofti kaugühenduvuse analüsaatorit](https://testconnectivity.microsoft.com/) ja käitage mõjutatud kasutaja jaoks **Microsoft Exchange’i veebiteenuste ühenduvuse testid**.

Lõpuks kontrollige [Teamsi rakenduste rakenduse häälestuspoliitikaid](https://admin.teams.microsoft.com/policies/app-setup), et tagada, et rakendus Kalender ei oleks kasutajale rakendatavast poliitikast eemaldatud (kõige tõenäolisemalt **globaalne (vaikimisi organisatsiooniülene)**.

Kui teie kasutajad on majutatud kohapeal, peate kinnitama, et teie hübriidkonfiguratsiooni seisund oleks hea. Kasutage tõrkeotsinguks [hübriidkonfiguratsiooni viisardit](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Pange tähele, et [Teamsi jaoks on vajalik Exchange 2016 CU3 või kõrgem](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
