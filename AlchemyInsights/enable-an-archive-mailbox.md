---
title: Arhiivi postkasti lubamine
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811701"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="9d152-102">Arhiivi postkasti lubamine</span><span class="sxs-lookup"><span data-stu-id="9d152-102">Enable an archive mailbox</span></span>

<span data-ttu-id="9d152-103">Kui soovite, et meil oleks võimalik konfigureerida automatiseeritud kontrolle, et tagada arhiivi postkasti häälestamine, valige nupp tagasi <--selle lehe ülaosas ja seejärel sisestage konto meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="9d152-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="9d152-104">Postkastide arhiivimine rakenduses Microsoft 365 (mida nimetatakse ka *Veebiarhiiviks* või *kohapealseks arhiivimiseks*) pakuvad kasutajatele täiendavaid salvestusruumi.</span><span class="sxs-lookup"><span data-stu-id="9d152-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="9d152-105">Kasutajad saavad üksusi arhiivi postkasti teisaldamiseks või kopeerimiseks ja administraatorid saavad luua arhiivimise poliitika, mis teisaldab üksused automaatselt postkastide arhiivi.</span><span class="sxs-lookup"><span data-stu-id="9d152-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="9d152-106">Arhiivi postkasti loomiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="9d152-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="9d152-107">Avage [https://protection.office.com](https://protection.office.com) .</span><span class="sxs-lookup"><span data-stu-id="9d152-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="9d152-108">Logige oma administraatori kontoga sisse rakendusse Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9d152-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="9d152-109">&amp;Valige turbe nõuetele vastavuse keskuse vasakul paanil **teave halduse** \> **arhiivimine**.</span><span class="sxs-lookup"><span data-stu-id="9d152-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="9d152-110">Valige kasutaja, kelle arhiivi postkasti soovite lubada.</span><span class="sxs-lookup"><span data-stu-id="9d152-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="9d152-111">Klõpsake paremal paanil üksikasjade paanil nuppu **Luba** ja seejärel nuppu **Jah** hoiatusteates, et lubada arhiivi postkast.</span><span class="sxs-lookup"><span data-stu-id="9d152-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="9d152-112">Samuti saate hulgi-lubada arhiivi postkastid, valides mitu kasutajat (kasutades **klahvikombinatsiooni SHIFT** või **Ctrl** ) ja klõpsates üksikasjade paanil nuppu **Luba** .</span><span class="sxs-lookup"><span data-stu-id="9d152-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="9d152-113">Ühiskasutatavad postkastid</span><span class="sxs-lookup"><span data-stu-id="9d152-113">Shared mailboxes</span></span>

<span data-ttu-id="9d152-114">Ühiskasutuses postkasti arhiivi lubamiseks on vaja Exchange Online ' i lepingu 2 litsentsi või Exchange Online ' i paketti, millel on Exchange Online ' i arhiivimiseks vajalik litsents.</span><span class="sxs-lookup"><span data-stu-id="9d152-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="9d152-115">Ühiskasutuses postkasti arhiivi lubamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="9d152-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="9d152-116">Avage [Exchange ' i halduskeskus](https://outlook.office365.com/ecp) ja logige sisse oma administraatorikonto abil.</span><span class="sxs-lookup"><span data-stu-id="9d152-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="9d152-117">Valige **Recipients**  >  **ühiskasutusse antud**adressaadid.</span><span class="sxs-lookup"><span data-stu-id="9d152-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="9d152-118">Valige Ühiskasutuses postkast.</span><span class="sxs-lookup"><span data-stu-id="9d152-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="9d152-119">Klõpsake paremal paanil üksikasjade paani jaotises **kohapealne Arhiiv**nuppu **Luba**ja seejärel arhiivi postkasti lubamiseks nuppu **Jah** .</span><span class="sxs-lookup"><span data-stu-id="9d152-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="9d152-120">Lisateavet leiate järgmisest teemast.</span><span class="sxs-lookup"><span data-stu-id="9d152-120">For more information, see:</span></span>
  
- [<span data-ttu-id="9d152-121">Luba arhiivi postkastid</span><span class="sxs-lookup"><span data-stu-id="9d152-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="9d152-122">Arhiivimise ja kustutamise poliitika häälestamine</span><span class="sxs-lookup"><span data-stu-id="9d152-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
