---
title: Väliste rühmade keelamine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704124"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="02a5d-102">Väliste rühmade keelamine</span><span class="sxs-lookup"><span data-stu-id="02a5d-102">How to disable External Groups</span></span>

<span data-ttu-id="02a5d-103">Yammeri väline sõnumside rakendab Exchange ' i transpordi reegleid (ETR), ennetavaid juhtelemente, et takistada ettevõtte andmete ühiskasutust.</span><span class="sxs-lookup"><span data-stu-id="02a5d-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="02a5d-104">Kui soovite, et kasutajad ei saaks väliseid rühmi luua, peate konfigureerima Exchange ' i transpordi reegli (ETR) ja seejärel konfigureerima Yammeri kasutama Exchange ' i transpordi reeglit väliste sõnumite blokeerimiseks.</span><span class="sxs-lookup"><span data-stu-id="02a5d-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="02a5d-105">Kui olete loonud reegli Exchange Online ' i administreerimiskeskuses, tehke Yammeri rakendamiseks ETR määramiseks järgmist.</span><span class="sxs-lookup"><span data-stu-id="02a5d-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="02a5d-106">Logige Yammerisse sisse kinnitatud administraatorina ja **Yammeri halduskeskus**, avage C- **sisu ja turbe turvasätted \> .**</span><span class="sxs-lookup"><span data-stu-id="02a5d-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="02a5d-107">Valige jaotises **väline sõnumside** **Yammeri kaudu oma Exchange Online ' i Exchange ' i transpordi reeglid (ETR).**</span><span class="sxs-lookup"><span data-stu-id="02a5d-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="02a5d-108">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="02a5d-108">Choose **Save**.</span></span>

<span data-ttu-id="02a5d-109">Lisateavet leiate teemast [väliste sõnumite keelamine Yammeri võrgus](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="02a5d-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  