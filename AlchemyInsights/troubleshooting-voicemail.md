---
title: 'Kõneposti tõrkeotsing '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677321"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="fdc44-102">Kõneposti tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="fdc44-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="fdc44-103">Veenduge, et hõivatud hõivatud funktsioon oleks tahtlik.</span><span class="sxs-lookup"><span data-stu-id="fdc44-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="fdc44-104">Kui see funktsioon pole selle kasutaja jaoks vajalik, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="fdc44-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="fdc44-105">Avage [meeskonnatöö halduskeskus](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="fdc44-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="fdc44-106">Vasakpoolsel rööpal Navigeerige **kõnede**  >  **poliitika**  >  **poliitikate haldamiseks** . </span><span class="sxs-lookup"><span data-stu-id="fdc44-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="fdc44-107">Valige **Halda kasutajaid**.</span><span class="sxs-lookup"><span data-stu-id="fdc44-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="fdc44-108">Kasutaja otsimine ja kõnepoliitika muutmine selliseks, mis on hõivatud hõivatud olekuga **, on saadaval ka kõne** **ajal.**</span><span class="sxs-lookup"><span data-stu-id="fdc44-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="fdc44-109">Klõpsake nuppu **Rakenda**.</span><span class="sxs-lookup"><span data-stu-id="fdc44-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="fdc44-110">Poliitikate muudatused võivad paljunemiseks kuluda kuni 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="fdc44-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="fdc44-111">Lisateavet selle funktsiooni kohta leiate järgmistest teemadest: [kõne ajal on saadaval hõivatud](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call)hõivatud.</span><span class="sxs-lookup"><span data-stu-id="fdc44-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
