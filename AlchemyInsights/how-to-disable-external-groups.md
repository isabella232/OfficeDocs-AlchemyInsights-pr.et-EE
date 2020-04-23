---
title: Välisrühmade keelamine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720764"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="e7c1b-102">Välisrühmade keelamine</span><span class="sxs-lookup"><span data-stu-id="e7c1b-102">How to disable External Groups</span></span>

<span data-ttu-id="e7c1b-103">Yammeri väline sõnumside rakendab Exchange transport reeglid (ETRs), ennetava juhtelementide kogum ettevõtte teabe ühiskasutamise vältimiseks.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="e7c1b-104">Selleks, et piirata kasutajatel luua väliseid rühmi, peate konfigureerima Exchange transport reegel (ETR) ja seejärel konfigureerige Yammeri kasutada Exchange transporti reegli blokeerida välise sõnumside.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="e7c1b-105">Kui olete loonud reegli Exchange Online ' i halduskeskus, toimige järgmiselt seada ETR rakendada Yammeri:</span><span class="sxs-lookup"><span data-stu-id="e7c1b-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="e7c1b-106">Yammeri sisse logida kontrollitud admin ja **Yammeri administreerimiskeskus**, C **sisu ja turvalisuse \> turvasätted.**</span><span class="sxs-lookup"><span data-stu-id="e7c1b-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="e7c1b-107">Jaotises **välise sõnumside**valige **jõustada Exchange Online ' i Exchange transport reeglid (Etrs) Yammeri.**</span><span class="sxs-lookup"><span data-stu-id="e7c1b-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="e7c1b-108">Valige käsk **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-108">Choose **Save**.</span></span>

<span data-ttu-id="e7c1b-109">Lisateabe saamiseks vaadake [Keela väline sõnumside Yammeri võrgus](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="e7c1b-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  