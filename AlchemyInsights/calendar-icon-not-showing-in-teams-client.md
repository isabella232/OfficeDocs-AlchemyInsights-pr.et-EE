---
title: Kalendri ikooni ei kuvata Teamsi klientrakenduses
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931981"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="2c64e-102">Kalendri ikooni ei kuvata Teamsi klientrakenduses</span><span class="sxs-lookup"><span data-stu-id="2c64e-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="2c64e-103">Teamsi vahekaart Kalender vajab Exchange’i veebiteenuste kaudu juurdepääsu Exchange’i postkastile.</span><span class="sxs-lookup"><span data-stu-id="2c64e-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="2c64e-104">Exchange’i postkast võib olla veebipõhine või kohapealne.</span><span class="sxs-lookup"><span data-stu-id="2c64e-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="2c64e-105">Veebiversiooni kasutajate puhul, kes vahekaarti Kalender ei näe, veenduge, et neil [oleks Exchange Online’i postkasti litsents ja postkast oleks lubatud](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="2c64e-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="2c64e-106">Kui kasutajal on Exchange Online’is kehtiv postkast, kuid nad endiselt vahekaarti Kalender ei näe, võib teil olla probleem võrguga.</span><span class="sxs-lookup"><span data-stu-id="2c64e-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="2c64e-107">Kasutage [Microsofti kaugühenduvuse analüsaatorit](https://testconnectivity.microsoft.com/) ja käitage mõjutatud kasutaja jaoks **Microsoft Exchange’i veebiteenuste ühenduvuse testid**.</span><span class="sxs-lookup"><span data-stu-id="2c64e-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="2c64e-108">Lõpuks kontrollige [Teamsi rakenduste rakenduse häälestuspoliitikaid](https://admin.teams.microsoft.com/policies/app-setup), et tagada, et rakendus Kalender ei oleks kasutajale rakendatavast poliitikast eemaldatud (kõige tõenäolisemalt **globaalne (vaikimisi organisatsiooniülene)**.</span><span class="sxs-lookup"><span data-stu-id="2c64e-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="2c64e-109">Kui teie kasutajad on majutatud kohapeal, peate kinnitama, et teie hübriidkonfiguratsiooni seisund oleks hea.</span><span class="sxs-lookup"><span data-stu-id="2c64e-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="2c64e-110">Kasutage tõrkeotsinguks [hübriidkonfiguratsiooni viisardit](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="2c64e-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="2c64e-111">Pange tähele, et [Teamsi jaoks on vajalik Exchange 2016 CU3 või kõrgem](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="2c64e-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
