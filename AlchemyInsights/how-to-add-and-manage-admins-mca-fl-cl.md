---
title: Kuidas lisada ja hallata administraatoritele – MCA FL/CL
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692113"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="e34bb-102">Kuidas lisada ja hallata administraatoritele – MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="e34bb-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="e34bb-103">Microsofti kliendi lepingu (MCA) arvelduse konto haldamiseks saate kasutada soovitud Accessi tasemega erinevaid rolle.</span><span class="sxs-lookup"><span data-stu-id="e34bb-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="e34bb-104">Need rollid on lisaks sisseehitatud Azure ' i teenuste rollidele, mis aitavad teil oma ressursse juhtida.</span><span class="sxs-lookup"><span data-stu-id="e34bb-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="e34bb-105">**Arvelduse rollide lisamiseks Azure ' i portaalis tehke järgmist.**</span><span class="sxs-lookup"><span data-stu-id="e34bb-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="e34bb-106">Logige sisse [Azure ' i portaali](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e34bb-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="e34bb-107">Otsige *kulude haldus + arveldus*.</span><span class="sxs-lookup"><span data-stu-id="e34bb-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="e34bb-108">Valige Access Control (IAM) ulatuses (nt arvelduse konto, arvelduse profiil või arve jaotis, kus soovite juurdepääsu anda.</span><span class="sxs-lookup"><span data-stu-id="e34bb-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="e34bb-109">Accessi juhtimise (IAM) lehel on loetletud kasutajad ja rühmad, kellele on määratud selle ulatuse iga roll.</span><span class="sxs-lookup"><span data-stu-id="e34bb-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="e34bb-110">Kasutajale juurdepääsu andmiseks valige lehe ülaservas nupp **Lisa** .</span><span class="sxs-lookup"><span data-stu-id="e34bb-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="e34bb-111">Valige ripploendis *roll* soovitud roll.</span><span class="sxs-lookup"><span data-stu-id="e34bb-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="e34bb-112">Sisestage selle kasutaja meiliaadress, kellele soovite juurdepääsu anda.</span><span class="sxs-lookup"><span data-stu-id="e34bb-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="e34bb-113">Rolli määramiseks valige **Salvesta** .</span><span class="sxs-lookup"><span data-stu-id="e34bb-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="e34bb-114">Kasutaja juurdepääsu eemaldamiseks valige selle rollimäärangu kasutaja, mille soovite eemaldada.</span><span class="sxs-lookup"><span data-stu-id="e34bb-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="e34bb-115">Valige **Eemalda**.</span><span class="sxs-lookup"><span data-stu-id="e34bb-115">Select **Remove**.</span></span>

<span data-ttu-id="e34bb-116">**Soovitatavad dokumendid**</span><span class="sxs-lookup"><span data-stu-id="e34bb-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="e34bb-117">Arvelduse rollide määratlused</span><span class="sxs-lookup"><span data-stu-id="e34bb-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="e34bb-118">Arvelduse konto rollid ja ülesanded</span><span class="sxs-lookup"><span data-stu-id="e34bb-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="e34bb-119">MCA arvelduse kontoga alustamine</span><span class="sxs-lookup"><span data-stu-id="e34bb-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="e34bb-120">Microsofti kliendi lepingule juurdepääsu kontrollimine</span><span class="sxs-lookup"><span data-stu-id="e34bb-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
