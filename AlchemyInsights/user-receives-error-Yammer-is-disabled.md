---
title: Kasutaja saab tõrke AADSTS7000112 Yammer on keelatud
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197872"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="ea7d4-102">Kasutaja saab tõrke AADSTS7000112 Yammer on keelatud</span><span class="sxs-lookup"><span data-stu-id="ea7d4-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="ea7d4-103">Kui kuvatakse tõrketeade "AADSTS7000112: rakendus '00000005-0000-0ff1-ce00-0000000000000"(Yammer) on keelatud", on probleem teenuse peamine Azure AD.-s.</span><span class="sxs-lookup"><span data-stu-id="ea7d4-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="ea7d4-104">Administraator võib olla keelanud teenuse subjekti Yammerile juurdepääsu blokeerimiseks.</span><span class="sxs-lookup"><span data-stu-id="ea7d4-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="ea7d4-105">Teenuse subjekti keelamine pole soovitatav ja võib põhjustada lisaprobleeme.</span><span class="sxs-lookup"><span data-stu-id="ea7d4-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="ea7d4-106">Lisateavet toetatud lähenemisviisi kohta, et blokeerida kasutajate juurdepääs Yammerile, leiate teemast [Yammeri juurdepääsu väljalülitamine Microsoft 365 kasutajatele](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="ea7d4-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="ea7d4-107">Azure'i portaali sprobleemi lahendamiseks ja yammerile kasutaja juurdepääsu taastamiseks</span><span class="sxs-lookup"><span data-stu-id="ea7d4-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="ea7d4-108">Avage leht Azure Active Directory ja valige vasakpoolsel navigeerimispaanil jaotises **Halda** suvand **Ettevõtte rakendused.**</span><span class="sxs-lookup"><span data-stu-id="ea7d4-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="ea7d4-109">Tippige otsinguväljale **Tekst Office 365 Yammer** ja valige sätete avamiseks rakenduse nimi.</span><span class="sxs-lookup"><span data-stu-id="ea7d4-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="ea7d4-110">Valige vasakpoolsel navigeerimispaanil jaotises **Halda** **suvand Atribuudid.**</span><span class="sxs-lookup"><span data-stu-id="ea7d4-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="ea7d4-111">Määrake suvandi **Lubatud kasutajatele sisselogimiseks väärtuseks** **Jah**ja seejärel valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="ea7d4-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="ea7d4-112">Logige uuesti Yammerisse sisse.</span><span class="sxs-lookup"><span data-stu-id="ea7d4-112">Sign in to Yammer again.</span></span> <span data-ttu-id="ea7d4-113">Võimalik, et peate küpsised kustutama.</span><span class="sxs-lookup"><span data-stu-id="ea7d4-113">You might need to clear cookies.</span></span>

<span data-ttu-id="ea7d4-114">Teise võimalusena käivitage PowerShelli käske väärtuse seadmiseks.</span><span class="sxs-lookup"><span data-stu-id="ea7d4-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="ea7d4-115">Lisateavet leiate teemast ["Kahju, kuid meil on probleeme sisselogimisega" tõrge, kui klõpsate Office 365 paani Yammer](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="ea7d4-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 