---
title: Kuidas keelata välised rühmad
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
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540897"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="4c101-102">Kuidas keelata välised rühmad</span><span class="sxs-lookup"><span data-stu-id="4c101-102">How to disable External Groups</span></span>

<span data-ttu-id="4c101-103">Yammeri välise sõnumside kehtib Exchange transpordireeglite (ETRs) komplekt ennetava kontrolli vältida ettevõtte andmed ühiselt.</span><span class="sxs-lookup"><span data-stu-id="4c101-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="4c101-104">Piirata, välised rühmad luua, peate konfigureerida Exchange Transpordireegli (ETR), ja seejärel konfigureerige Yammeri blokeerida välist sõnumid Exchange Transpordireegli abil.</span><span class="sxs-lookup"><span data-stu-id="4c101-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="4c101-105">Kui reegel on loodud Exchange Online'i administreerimiskeskuses, toimige järgnevalt, et seada ETR Yammeri kohaldada</span><span class="sxs-lookup"><span data-stu-id="4c101-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="4c101-106">Logige Yammeri ehtsat admin ja **Yammer halduskeskus**, Mine C **sisu ja turvalisuse \> turvasätted.**</span><span class="sxs-lookup"><span data-stu-id="4c101-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="4c101-107">**Välise sõnumside**, valige **jõustada teie Exchange Online Exchange transpordireeglite (ETRs) Yammeri.**</span><span class="sxs-lookup"><span data-stu-id="4c101-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="4c101-108">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="4c101-108">Choose **Save**.</span></span>

<span data-ttu-id="4c101-109">Lisateabe saamiseks vaadake teemat [kontrolli välise sõnumid Exchange transpordireeglite Yammeri võrgustiku](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="4c101-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  