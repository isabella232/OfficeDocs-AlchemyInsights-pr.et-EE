---
title: 126 Kas OWA-s ei leita postkasti saamist?
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
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426658"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="be92c-102">Kas Outlooki veebirakenduses ei leitud postkasti tõrkeid?</span><span class="sxs-lookup"><span data-stu-id="be92c-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="be92c-103">Kui kasutate Outlooki veebirakendust ja tõrketeadet  postkasti ei leitud, pole kontol, mida kasutasite Outlooki veebirakendusega ühenduse loomiseks, Exchange Online'i litsentsi ja seetõttu pole kontoga seotud ühtegi postkasti.</span><span class="sxs-lookup"><span data-stu-id="be92c-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="be92c-104">Teie administraator saab teie kontole litsentsi määrata, järgides järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="be92c-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="be92c-105">Avage [Microsoft 365 halduskeskus](https://portal.office.com/adminportal/home#/homepage)  ja avage  jaotises Kasutajad jaotis Aktiivsed kasutajad ja valige kasutaja, kes seda tõrget näeb.</span><span class="sxs-lookup"><span data-stu-id="be92c-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="be92c-106">Avage avalehel jaotis Litsentsid **ja** rakendused, valige sobiv  väärtus Asukoht ja määrake litsents, mis sisaldab Exchange Online'i (litsentsi üksikasjade määramiseks laiendage litsentsi).</span><span class="sxs-lookup"><span data-stu-id="be92c-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="be92c-107">Kui olete lõpetanud, klõpsake nuppu **Salvesta muudatused.**</span><span class="sxs-lookup"><span data-stu-id="be92c-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="be92c-108">Mõnel juhul, kui litsents on juba kasutajakontole määratud, aitab litsentsi eemaldamine ja ümbermääramine probleemi lahendada ja seda süsteemis õigesti ette ettevalmistamise abil ette näha.</span><span class="sxs-lookup"><span data-stu-id="be92c-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="be92c-109">Kontrollige, kas teie M365 Exchange Online'i (ja muud, kui teil on) tellimused on praegused ja pole hiljuti aegunud.</span><span class="sxs-lookup"><span data-stu-id="be92c-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="be92c-110">Kui olete veendunud, et teie tellimus pole aegunud ja kasutajakontole on määratud kehtiv litsents, võib tellimuse ettevalmistamine võtta kuni 24 tundi, nii et peate võib-olla ootama, kuni probleem laheneks.</span><span class="sxs-lookup"><span data-stu-id="be92c-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="be92c-111">Lisateavet leiate teemast [Litsentside määramine ja haldamine.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="be92c-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>