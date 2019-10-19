---
title: Välisrühmade keelamine
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36739489"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="70668-102">Välisrühmade keelamine</span><span class="sxs-lookup"><span data-stu-id="70668-102">How to disable External Groups</span></span>

<span data-ttu-id="70668-103">Yammeri väline sõnumside rakendab Exchange transport reeglid (ETRs), ennetava juhtelementide kogum ettevõtte teabe ühiskasutamise vältimiseks.</span><span class="sxs-lookup"><span data-stu-id="70668-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="70668-104">Selleks, et piirata kasutajatel luua väliseid rühmi, peate konfigureerima Exchange transport reegel (ETR) ja seejärel konfigureerige Yammeri kasutada Exchange transporti reegli blokeerida välise sõnumside.</span><span class="sxs-lookup"><span data-stu-id="70668-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="70668-105">Kui olete loonud reegli Exchange Online ' i halduskeskus, toimige järgmiselt seada ETR rakendada Yammeri:</span><span class="sxs-lookup"><span data-stu-id="70668-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="70668-106">Yammeri sisse logida kontrollitud admin ja **Yammeri administreerimiskeskus**, minge C **sisu ja turvalisuse \> turvasätted.**</span><span class="sxs-lookup"><span data-stu-id="70668-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="70668-107">Jaotises **välise sõnumside**valige **jõustada Exchange Online ' i Exchange transport reeglid (Etrs) Yammeri.**</span><span class="sxs-lookup"><span data-stu-id="70668-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="70668-108">Valige käsk **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="70668-108">Choose **Save**.</span></span>

<span data-ttu-id="70668-109">Lisateabe saamiseks vaadake [Keela väline sõnumside Yammeri võrgus](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="70668-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  