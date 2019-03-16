---
title: Outlooki töölaua tagasikutsumine või asendamine e-kirja
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657040"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="c3930-102">Tagasi kutsuda või asendada e-kirja</span><span class="sxs-lookup"><span data-stu-id="c3930-102">Recall or replace an email message</span></span>

- <span data-ttu-id="c3930-103">Admin, võite **meenutavad sõnumid PowerShelli abil kasutajate nimel**.</span><span class="sxs-lookup"><span data-stu-id="c3930-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="c3930-104">Ei mäleta sõnumeid halduskeskuse kaudu.</span><span class="sxs-lookup"><span data-stu-id="c3930-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="c3930-105">Saab **ainult turult sõnumid, mis saadetakse ettevõtte**.</span><span class="sxs-lookup"><span data-stu-id="c3930-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="c3930-106">Kui sõnum saadeti Gmaili aadressi, näiteks ei mäleta seda.</span><span class="sxs-lookup"><span data-stu-id="c3930-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="c3930-107">Saab **ainult turult kirjad Outlook 2016 PC**.</span><span class="sxs-lookup"><span data-stu-id="c3930-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="c3930-108">Kui kasutaja saadab sõnumi, kasutades Outlook for Mac või Outlook veebis, ei mäleta seda.</span><span class="sxs-lookup"><span data-stu-id="c3930-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="c3930-109">Tagasikutsumise või asendamise e-kirja:</span><span class="sxs-lookup"><span data-stu-id="c3930-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="c3930-110">Valige Outlooki vasakul paanil kausta kausta Saadetud.</span><span class="sxs-lookup"><span data-stu-id="c3930-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="c3930-111">Topeltklõpsake selle avamiseks tagasi kutsutava.</span><span class="sxs-lookup"><span data-stu-id="c3930-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="c3930-112">Valige **sõnum** jaotises ja seejärel valige **toiminguid** > **Kutsu see sõnum tagasi**.</span><span class="sxs-lookup"><span data-stu-id="c3930-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="c3930-113">Valige **kustutada selle sõnumi lugemata eksemplarid** või **kustutada lugemata eksemplarid ja asendada need uue sõnumiga**ja seejärel klõpsake **nuppu OK**.</span><span class="sxs-lookup"><span data-stu-id="c3930-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="c3930-114">Asendamine sõnumi saatmisel Koosta sõnum ja valige **saada**.</span><span class="sxs-lookup"><span data-stu-id="c3930-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="c3930-115">Sõnumi tagasikutsumise takistavaid sõltub teenuse kasutaja Outlooki sätteid.</span><span class="sxs-lookup"><span data-stu-id="c3930-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="c3930-116">Kontrollida tόhistamise kohta leiate [käesoleva artikli](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="c3930-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="c3930-117">Otsida ja kustutada e-kirju teie organisatsiooni</span><span class="sxs-lookup"><span data-stu-id="c3930-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="c3930-118">Kui sa ei ole globaalne admin, lisatakse teie konto e-juurdluse haldur rolli või vastavuse Otsi rollirühma otsida sõnumeid.</span><span class="sxs-lookup"><span data-stu-id="c3930-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="c3930-119">Sõnumite kustutamiseks peate organisatsioonihalduse rollirühma või otsingu- ja Likvideeri RBAC-roll.</span><span class="sxs-lookup"><span data-stu-id="c3930-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="c3930-120">Nende rollide õiguste määratakse [Turve ja vastavus center](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="c3930-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="c3930-121">[Loo sisu otsida](https://docs.microsoft.com/office365/securitycompliance/content-search) leida sõnumi kustutamiseks.</span><span class="sxs-lookup"><span data-stu-id="c3930-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="c3930-122">[Turvalisus ja vastavus Center PowerShelli](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="c3930-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="c3930-123">Mitmekordne autentimine kasutamisel vaadake [ühenduse loomine Office 365 turvalisuse ja nõuetele vastavuse Center PowerShelli kasutamine mitmefaktorilist autentimist](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="c3930-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>