---
title: Outlooki töölaua tagasivõtmine või asendamine e-kirja
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502315"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="e4542-102">Outlooki e-kirja tagasivõtmine või asendamine</span><span class="sxs-lookup"><span data-stu-id="e4542-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="e4542-103">Nagu admin, saate **meenutada sõnumeid kasutajate nimel, kasutades PowerShelli**.</span><span class="sxs-lookup"><span data-stu-id="e4542-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="e4542-104">Administreerimiskeskusest ei saa sõnumeid meenutada.</span><span class="sxs-lookup"><span data-stu-id="e4542-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="e4542-105">Te saate **ainult meenutada sõnumeid, mis saadetakse inimestele teie organisatsioonis**.</span><span class="sxs-lookup"><span data-stu-id="e4542-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="e4542-106">Kui sõnum saadeti näiteks Gmaili aadressile, ei saa te seda meenutada.</span><span class="sxs-lookup"><span data-stu-id="e4542-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="e4542-107">Võite **meenutada ainult sõnumeid, mis on saadetud Outlook 2016 arvutist**.</span><span class="sxs-lookup"><span data-stu-id="e4542-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="e4542-108">Kui kasutaja saadab sõnumi, kasutades Outlook for Mac või Outlook veebis, ei mäleta seda.</span><span class="sxs-lookup"><span data-stu-id="e4542-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="e4542-109">E-kirja tagasikutsumiseks või asendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="e4542-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="e4542-110">Valige Outlooki aknast vasakul asuva kaustapaanil kaust saadetud.</span><span class="sxs-lookup"><span data-stu-id="e4542-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="e4542-111">Selle avamiseks topeltklõpsake sõnumit, mida soovite meenutada.</span><span class="sxs-lookup"><span data-stu-id="e4542-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="e4542-112">Valige vahekaart **sõnum** ja seejärel valige suvand **Tegevused**  >  **Meenuta seda sõnumit**.</span><span class="sxs-lookup"><span data-stu-id="e4542-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="e4542-113">Valige **kustutage selle sõnumi lugemata koopiad** või **kustutage lugemata koopiad ja asendage see uue sõnumiga**ning valige seejärel **OK**.</span><span class="sxs-lookup"><span data-stu-id="e4542-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="e4542-114">Kui saadate asendussõnumi, koostage sõnum ja valige siis **saada**.</span><span class="sxs-lookup"><span data-stu-id="e4542-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="e4542-115">Sõnumi tagasikutsumise õnnestumine või nurjumine sõltub adressaadi sätetest Outlookis.</span><span class="sxs-lookup"><span data-stu-id="e4542-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="e4542-116">Juhised tagasivõtmist kontrollida, vt [käesoleva artikli](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="e4542-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="e4542-117">Meilisõnumite otsimine ja kustutamine teie organisatsioonis</span><span class="sxs-lookup"><span data-stu-id="e4542-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="e4542-118">Kui te pole globaalne administraator, tuleb teie konto lisada eDiscovery Manageri rollile või vastavuse otsingu haldamise rollile sõnumite otsimiseks.</span><span class="sxs-lookup"><span data-stu-id="e4542-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="e4542-119">Sõnumite kustutamiseks peate liituma organisatsiooni juhtimise rolligrupiga või otsingu ja Purge juhtimise rolliga.</span><span class="sxs-lookup"><span data-stu-id="e4542-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="e4542-120">Nende rollide õigused määratakse [turbe-ja Vastavuskeskuses](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="e4542-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="e4542-121">[Saate luua sisuotsingu](https://docs.microsoft.com/microsoft-365/compliance/content-search) , et leida kustutatav sõnum.</span><span class="sxs-lookup"><span data-stu-id="e4542-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="e4542-122">[Ühendage turbe-ja Vastavuskeskus PowerShelli](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="e4542-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="e4542-123">Kui kasutate mitme teguriga autentimine, vaadake [ühendust Microsoft 365 turvalisuse ja vastavuse Center PowerShelli mitme teguriga autentimine abil](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="e4542-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>