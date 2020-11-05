---
title: Azure ' i arvelduse omaniku üleviimine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922074"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="bc9c5-102">Azure ' i arvelduse omaniku üleviimine</span><span class="sxs-lookup"><span data-stu-id="bc9c5-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="bc9c5-103">Logige [Azure ' i portaali](https://portal.azure.com/) sisse selle tellimuse administraatorina, mille soovite üle viia.</span><span class="sxs-lookup"><span data-stu-id="bc9c5-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="bc9c5-104">Kui te pole kindel, kas olete administraator, või peate tuvastama, kes on, lugege teemat [konto arvelduse halduri määramine](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="bc9c5-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="bc9c5-105">Otsige **kulude haldus + arveldus**.</span><span class="sxs-lookup"><span data-stu-id="bc9c5-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="bc9c5-106">Valige vasakult paanilt **tellimused** .</span><span class="sxs-lookup"><span data-stu-id="bc9c5-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="bc9c5-107">Olenevalt Accessist peate võib-olla valima arveldamise ulatuse ja seejärel **tellimused** või **Azure ' i tellimused**.</span><span class="sxs-lookup"><span data-stu-id="bc9c5-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="bc9c5-108">Valige üle kantava tellimuse **ülekandmise arveldamise omanik**</span><span class="sxs-lookup"><span data-stu-id="bc9c5-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="bc9c5-109">Sisestage selle kasutaja meiliaadress, kes on tellimuse uueks omanikuks oleva konto arveldamise administraator ja seejärel valige **saada edastuse taotlus**</span><span class="sxs-lookup"><span data-stu-id="bc9c5-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="bc9c5-110">Kasutaja saab teie edastuse taotluse läbivaatamiseks meili teel juhiseid.</span><span class="sxs-lookup"><span data-stu-id="bc9c5-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="bc9c5-111">Edastuse taotluse kinnitamiseks valib kasutaja meilisõnumis oleva lingi ja järgib juhiseid.</span><span class="sxs-lookup"><span data-stu-id="bc9c5-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="bc9c5-112">**Märkus** : Kui edastate oma tellimuse arveldamise omandiõiguse mõnele teisele Azure AD rentniku kontole, eemaldatakse kõik [rolli-põhise juurdepääsu juhtimise (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)ülesanded tellimuse ressursside haldamiseks jäädavalt.</span><span class="sxs-lookup"><span data-stu-id="bc9c5-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="bc9c5-113">Ainult uuel omanikul on juurdepääs tellimuse ressursside haldamiseks.</span><span class="sxs-lookup"><span data-stu-id="bc9c5-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="bc9c5-114">Lisateavet leiate teemast [tellimuse edastamine kasutajale teise AZURE ad rentniku](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)jaoks.</span><span class="sxs-lookup"><span data-stu-id="bc9c5-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="bc9c5-115">**Soovitatavad dokumendid**</span><span class="sxs-lookup"><span data-stu-id="bc9c5-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="bc9c5-116">Azure ' i tellimuse arveldamise omandiõiguse üleviimine teisele kontole</span><span class="sxs-lookup"><span data-stu-id="bc9c5-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="bc9c5-117">Arvelduse omandiõiguse üleminek Azure ' i tellimusele</span><span class="sxs-lookup"><span data-stu-id="bc9c5-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="bc9c5-118">Üle Visual Studio, Microsoft Partner Network (MPN) ja maksta, kui lähete dev/test tellimused</span><span class="sxs-lookup"><span data-stu-id="bc9c5-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="bc9c5-119">Omandiõiguse ülekandmise KKK</span><span class="sxs-lookup"><span data-stu-id="bc9c5-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="bc9c5-120">Omandiõiguse ülekandmise probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="bc9c5-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
