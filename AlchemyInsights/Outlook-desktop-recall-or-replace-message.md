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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389675"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="7eec1-102">Tagasi kutsuda või asendada e-kirja</span><span class="sxs-lookup"><span data-stu-id="7eec1-102">Recall or replace an email message</span></span>

- <span data-ttu-id="7eec1-103">Admin, võite **meenutavad sõnumid PowerShelli abil kasutajate nimel**.</span><span class="sxs-lookup"><span data-stu-id="7eec1-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="7eec1-104">Ei mäleta sõnumeid halduskeskuse kaudu.</span><span class="sxs-lookup"><span data-stu-id="7eec1-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="7eec1-105">Saab **ainult turult sõnumid, mis saadetakse ettevõtte**.</span><span class="sxs-lookup"><span data-stu-id="7eec1-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="7eec1-106">Kui sõnum saadeti Gmaili aadressi, näiteks ei mäleta seda.</span><span class="sxs-lookup"><span data-stu-id="7eec1-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="7eec1-107">Saab **ainult turult kirjad Outlook 2016 PC**.</span><span class="sxs-lookup"><span data-stu-id="7eec1-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="7eec1-108">Kui kasutaja saadab sõnumi, kasutades Outlook for Mac või Outlook veebis, ei mäleta seda.</span><span class="sxs-lookup"><span data-stu-id="7eec1-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="7eec1-109">Tagasikutsumise või asendamise e-kirja:</span><span class="sxs-lookup"><span data-stu-id="7eec1-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="7eec1-110">Valige Outlooki vasakul paanil kausta kausta Saadetud.</span><span class="sxs-lookup"><span data-stu-id="7eec1-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="7eec1-111">Topeltklõpsake selle avamiseks tagasi kutsutava.</span><span class="sxs-lookup"><span data-stu-id="7eec1-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="7eec1-112">Valige **sõnum** jaotises ja seejärel valige **toiminguid** > **Kutsu see sõnum tagasi**.</span><span class="sxs-lookup"><span data-stu-id="7eec1-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="7eec1-113">Valige **kustutada selle sõnumi lugemata eksemplarid** või **kustutada lugemata eksemplarid ja asendada need uue sõnumiga**ja seejärel klõpsake **nuppu OK**.</span><span class="sxs-lookup"><span data-stu-id="7eec1-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="7eec1-114">Asendamine sõnumi saatmisel Koosta sõnum ja valige **saada**.</span><span class="sxs-lookup"><span data-stu-id="7eec1-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="7eec1-115">Sõnumi tagasikutsumise takistavaid sõltub teenuse kasutaja Outlooki sätteid.</span><span class="sxs-lookup"><span data-stu-id="7eec1-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="7eec1-116">Kontrollida tόhistamise kohta leiate [käesoleva artikli](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="7eec1-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="7eec1-117">Otsida ja kustutada e-kirju teie organisatsiooni</span><span class="sxs-lookup"><span data-stu-id="7eec1-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="7eec1-118">Kui sa ei ole globaalne admin, lisatakse teie konto e-juurdluse haldur rolli või vastavuse Otsi rollirühma otsida sõnumeid.</span><span class="sxs-lookup"><span data-stu-id="7eec1-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="7eec1-119">Sõnumite kustutamiseks peate organisatsioonihalduse rollirühma või otsingu- ja Likvideeri RBAC-roll.</span><span class="sxs-lookup"><span data-stu-id="7eec1-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="7eec1-120">Nende rollide õiguste määratakse [Turve ja vastavus center](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="7eec1-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="7eec1-121">[Loo sisu otsida](https://docs.microsoft.com/office365/securitycompliance/content-search) leida sõnumi kustutamiseks.</span><span class="sxs-lookup"><span data-stu-id="7eec1-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="7eec1-122">[Turvalisus ja vastavus Center PowerShelli](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7eec1-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="7eec1-123">Mitmekordne autentimine kasutamisel vaadake [ühenduse loomine Office 365 turvalisuse ja nõuetele vastavuse Center PowerShelli kasutamine mitmefaktorilist autentimist](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7eec1-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>