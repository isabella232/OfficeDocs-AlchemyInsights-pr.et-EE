---
title: 126 kuidas postkastist ei leita tõrget OWA-s?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706746"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="9d733-102">Kas postkasti ei leitud Outlooki veebirakenduses viga?</span><span class="sxs-lookup"><span data-stu-id="9d733-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="9d733-103">Kui kasutate Outlooki veebirakenduses ja te **ei leia postkasti tõrke eest** , siis konto, mida kasutasite Outlooki veebirakendusega ühenduse loomiseks, ei sisalda Exchange Online ' i litsentsi ja seetõttu pole kontoga seotud ühtegi postkasti.</span><span class="sxs-lookup"><span data-stu-id="9d733-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="9d733-104">Teie administraator saab teie kontole litsentsi määrata, järgides järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="9d733-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="9d733-105">Avage [Microsoft 365 halduskeskus](https://portal.office.com/adminportal/home#/homepage) ja liikuge jaotise **Kasutajad jaotises kasutajad** **aktiivsetele kasutajatele** ja valige tõrget kuvav kasutaja.</span><span class="sxs-lookup"><span data-stu-id="9d733-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="9d733-106">Avage avanevas kasutajate lehel jaotis **litsentsid ja rakendused** , valige sobiv **asukoha** väärtus ja määrake Exchange Online ' i sisaldav litsents (laiendage litsentsi, et näha selle üksikasju).</span><span class="sxs-lookup"><span data-stu-id="9d733-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="9d733-107">Kui olete lõpetanud, klõpsake nuppu **Salvesta muudatused**.</span><span class="sxs-lookup"><span data-stu-id="9d733-107">When you're finished, click **Save changes**.</span></span>
