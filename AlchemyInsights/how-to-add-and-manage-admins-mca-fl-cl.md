---
title: Administraatorite lisamine ja haldamine
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
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755435"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="c0896-102">Administraatorite lisamine ja haldamine</span><span class="sxs-lookup"><span data-stu-id="c0896-102">How to add and manage admins</span></span>

<span data-ttu-id="c0896-103">Teie probleemi kirjelduse põhjal oleme leidnud teile lahenduse.</span><span class="sxs-lookup"><span data-stu-id="c0896-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="c0896-104">Enamik kliente suutsid oma probleemi lahendada pärast meie dokumentide järgimist.</span><span class="sxs-lookup"><span data-stu-id="c0896-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="c0896-105">Microsofti kliendi lepingu (MCA) arvelduse konto haldamiseks saate kasutada soovitud Accessi tasemega erinevaid rolle.</span><span class="sxs-lookup"><span data-stu-id="c0896-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="c0896-106">Need rollid on lisaks sisseehitatud Azure ' i teenuste rollidele, mis aitavad teil oma ressursse juhtida.</span><span class="sxs-lookup"><span data-stu-id="c0896-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="c0896-107">**Arvelduse rollide lisamiseks Azure ' i portaalis tehke järgmist.**</span><span class="sxs-lookup"><span data-stu-id="c0896-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="c0896-108">Logige sisse [Azure ' i portaali](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c0896-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="c0896-109">Otsige *kulude haldus + arveldus*.</span><span class="sxs-lookup"><span data-stu-id="c0896-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="c0896-110">Valige Access Control (IAM) ulatuses (nt arvelduse konto, arvelduse profiil või arve jaotis, kus soovite juurdepääsu anda.</span><span class="sxs-lookup"><span data-stu-id="c0896-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="c0896-111">Accessi juhtimise (IAM) lehel on loetletud kasutajad ja rühmad, kellele on määratud selle ulatuse iga roll.</span><span class="sxs-lookup"><span data-stu-id="c0896-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="c0896-112">Kasutajale juurdepääsu andmiseks valige lehe ülaservas nupp **Lisa** .</span><span class="sxs-lookup"><span data-stu-id="c0896-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="c0896-113">Valige ripploendis *roll* soovitud roll.</span><span class="sxs-lookup"><span data-stu-id="c0896-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="c0896-114">Sisestage selle kasutaja meiliaadress, kellele soovite juurdepääsu anda.</span><span class="sxs-lookup"><span data-stu-id="c0896-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="c0896-115">Rolli määramiseks valige **Salvesta** .</span><span class="sxs-lookup"><span data-stu-id="c0896-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="c0896-116">Kasutaja juurdepääsu eemaldamiseks valige selle rollimäärangu kasutaja, mille soovite eemaldada.</span><span class="sxs-lookup"><span data-stu-id="c0896-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="c0896-117">Valige **Eemalda**.</span><span class="sxs-lookup"><span data-stu-id="c0896-117">Select **Remove**.</span></span>

<span data-ttu-id="c0896-118">**Soovitatud dokumendid**</span><span class="sxs-lookup"><span data-stu-id="c0896-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="c0896-119">Arvelduse rollide määratlused</span><span class="sxs-lookup"><span data-stu-id="c0896-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="c0896-120">Arvelduse konto rollid ja ülesanded</span><span class="sxs-lookup"><span data-stu-id="c0896-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="c0896-121">MCA arvelduse kontoga alustamine</span><span class="sxs-lookup"><span data-stu-id="c0896-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="c0896-122">Microsofti kliendi lepingule juurdepääsu kontrollimine</span><span class="sxs-lookup"><span data-stu-id="c0896-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
