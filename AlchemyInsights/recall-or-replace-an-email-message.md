---
title: Meilisõnumi tagasikutsumine või asendamine
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353502"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="509c9-102">Meilisõnumi tagasikutsumine või asendamine rakenduses Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="509c9-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="509c9-103">Saate tagasi **kutsuda ainult teie asutuse inimestele saadetud sõnumeid**.</span><span class="sxs-lookup"><span data-stu-id="509c9-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="509c9-104">Näiteks kui sõnum saadeti Gmaili aadressile, ei saa te seda meelde tuletada.</span><span class="sxs-lookup"><span data-stu-id="509c9-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="509c9-105">Saate tagasi **kutsuda ainult Outlooki arvutist saadetud sõnumeid**.</span><span class="sxs-lookup"><span data-stu-id="509c9-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="509c9-106">Kui kasutaja saadab Outlook for Maci või Outlooki veebirakenduse kaudu sõnumi, ei saa seda enam meelde tuletada.</span><span class="sxs-lookup"><span data-stu-id="509c9-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="509c9-107">Rentniku administraatorina saate **kasutajate nimel sõnumeid tagasi kutsuda PowerShelli abil** (Lisateavet leiate teemast meilisõnumite [otsimine ja kustutamine](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="509c9-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="509c9-108">Administreerimiskeskuse sõnumeid ei saa tagasi kutsuda.</span><span class="sxs-lookup"><span data-stu-id="509c9-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="509c9-109">Lisateavet leiate jaotisest "oma asutuse meilisõnumite otsimine ja kustutamine".</span><span class="sxs-lookup"><span data-stu-id="509c9-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="509c9-110">**Saadetud meilisõnumi tagasivõtmine või asendamine**</span><span class="sxs-lookup"><span data-stu-id="509c9-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="509c9-111">Valige Outlooki akna vasakus servas asuval paanil kaust saadetud üksused.</span><span class="sxs-lookup"><span data-stu-id="509c9-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="509c9-112">Avage sõnum, mille soovite tagasi kutsuda.</span><span class="sxs-lookup"><span data-stu-id="509c9-112">Open the message that you want to recall.</span></span> <span data-ttu-id="509c9-113">Sõnumi avamiseks peate seda topeltklõpsama.</span><span class="sxs-lookup"><span data-stu-id="509c9-113">You must double-click to open the message.</span></span> <span data-ttu-id="509c9-114">Sõnumi valimine lugemispaanil kuvamisel ei luba teil sõnumit tagasi kutsuda.</span><span class="sxs-lookup"><span data-stu-id="509c9-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="509c9-115">Valige menüü Sõnum käsk **toimingud**, mida  >  **see sõnum tagasi kutsuda**.</span><span class="sxs-lookup"><span data-stu-id="509c9-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="509c9-116">Valige **Kustuta selle sõnumi lugemata eksemplarid** või **Kustuta lugemata eksemplarid ja asendage see uue sõnumiga**, seejärel valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="509c9-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="509c9-117">Kui saadate asendus-sõnumi, koostage sõnum ja seejärel valige **saada**.</span><span class="sxs-lookup"><span data-stu-id="509c9-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="509c9-118">Sõnumi tagasivõtmise õnnestumine või ebaõnnestumine sõltub Outlooki adressaatide sätetest.</span><span class="sxs-lookup"><span data-stu-id="509c9-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="509c9-119">Lisateavet (sh tagasivõtmine) leiate teemast saadetud meilisõnumi [tagasikutsumine või asendamine](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="509c9-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="509c9-120">**_Oma asutuses meilisõnumite otsimiseks ja kustutamiseks_** on see lihtsaim viis, kui olete globaalne administraator. Kui te pole üldadministraator, peab teie konto olema lisatud e-juurdluse halduri rollirühma või vastavuse otsingu juhtimise rollile.</span><span class="sxs-lookup"><span data-stu-id="509c9-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="509c9-121">Sõnumite kustutamiseks peate liituma organisatsiooni juhtimise rollirühma või otsingu ja likvideerimise rolliga.</span><span class="sxs-lookup"><span data-stu-id="509c9-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="509c9-122">Nende rollide kasutusõigused määratakse [turbe & täitmise keskuses](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="509c9-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="509c9-123">[Saate luua sisu otsimise](https://docs.microsoft.com/microsoft-365/compliance/content-search) , et leida sõnum, mille soovite kustutada.</span><span class="sxs-lookup"><span data-stu-id="509c9-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="509c9-124">[Looge ühendus turbe & vastavuse keskusega PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="509c9-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="509c9-125">Kui kasutate MFA-d (mitme teguriga autentimine), lugege teemat [ühenduse loomine Microsoft 365 turbe & nõuetele vastavuse keskus PowerShelli abil mitme teguriga autentimine](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="509c9-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
