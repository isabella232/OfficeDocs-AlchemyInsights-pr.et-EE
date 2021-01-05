---
title: Administraatorite lisamine ja haldamine – Soovitatavad juhised
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755831"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="06976-102">Administraatorite lisamine ja haldamine – Soovitatavad juhised</span><span class="sxs-lookup"><span data-stu-id="06976-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="06976-103">Teie probleemi kirjelduse põhjal oleme leidnud teile lahenduse.</span><span class="sxs-lookup"><span data-stu-id="06976-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="06976-104">Enamik kliente suutsid oma probleemi lahendada pärast meie dokumentide järgimist.</span><span class="sxs-lookup"><span data-stu-id="06976-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="06976-105">**Tellimuse halduri või koostöö administraatori redigeerimine**</span><span class="sxs-lookup"><span data-stu-id="06976-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="06976-106">Konto administraator saab redigeerida mõlemat rolli, samas kui tellimuse administraator saab [Azure ' i portaalis](https://ms.portal.azure.com/#home)ainult administraatoreid muuta.</span><span class="sxs-lookup"><span data-stu-id="06976-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="06976-107">Azure ' i tellimuse administraatorite lisamine või muutmine</span><span class="sxs-lookup"><span data-stu-id="06976-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="06976-108">**Tellimuse halduri või Co-Administrator sise (PÜSTI) tellimuste värskendamine**</span><span class="sxs-lookup"><span data-stu-id="06976-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="06976-109">Teenuse administraator või administraator saab seda toimingut ise teenida järgmiste toimingute abil.</span><span class="sxs-lookup"><span data-stu-id="06976-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="06976-110">Logige sisse [Azure ' i portaali](https://ms.portal.azure.com/#home) ja klõpsake vasakpoolsel Blade ' is nuppu **kulude haldus + arveldus** .</span><span class="sxs-lookup"><span data-stu-id="06976-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="06976-111">Klõpsake oma tellimusel rea üksust.</span><span class="sxs-lookup"><span data-stu-id="06976-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="06976-112">See avab teie tellimuse ülevaate.</span><span class="sxs-lookup"><span data-stu-id="06976-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="06976-113">Klõpsake **tellimuse** laba nuppu **Atribuudid**.</span><span class="sxs-lookup"><span data-stu-id="06976-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="06976-114">Klõpsake nuppu **teenuse administraator** .</span><span class="sxs-lookup"><span data-stu-id="06976-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="06976-115">Sisestage selle kasutaja meiliaadress, kelle soovite määrata teenuse administraatoriks, ja klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="06976-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="06976-116">**Lisa/Muuda/Eemalda kaas-administraator**</span><span class="sxs-lookup"><span data-stu-id="06976-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="06976-117">Logige [Azure ' i portaali](https://ms.portal.azure.com/#home) sisse teenuse administraatorina.</span><span class="sxs-lookup"><span data-stu-id="06976-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="06976-118">Avage [tellimused](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ja valige pakett.</span><span class="sxs-lookup"><span data-stu-id="06976-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="06976-119">(Adminstrators saab määrata ainult tellimuse ulatuses.)</span><span class="sxs-lookup"><span data-stu-id="06976-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="06976-120">Navigeerige **Accessi juhtelementi (iam)**  >  **klassikalised administraatorid**  >  **Lisa** kaas-  >  administraatori paani avamiseks lisa  **kaas-administraator** (kui suvand Lisa kaas-administraator on keelatud, tähendab see, et teil pole õigust).</span><span class="sxs-lookup"><span data-stu-id="06976-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="06976-121">Valige kasutaja, kelle soovite lisada, ja klõpsake nuppu **Lisa**.</span><span class="sxs-lookup"><span data-stu-id="06976-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="06976-122">**Lisateave:**</span><span class="sxs-lookup"><span data-stu-id="06976-122">**Learn more:**</span></span>
- [<span data-ttu-id="06976-123">Lisa kaas-administraator</span><span class="sxs-lookup"><span data-stu-id="06976-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="06976-124">Administraatori eemaldamine</span><span class="sxs-lookup"><span data-stu-id="06976-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="06976-125">Teenuse administraatori muutmine</span><span class="sxs-lookup"><span data-stu-id="06976-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="06976-126">Konto halduri kuvamine</span><span class="sxs-lookup"><span data-stu-id="06976-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="06976-127">Accessi haldamine RBAC ja Azure ' i portaali kaudu</span><span class="sxs-lookup"><span data-stu-id="06976-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="06976-128">**Kasutajate lisamine ja kustutamine Azure Active Directory abil (AD)**</span><span class="sxs-lookup"><span data-stu-id="06976-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="06976-129">Saate lisada uusi kasutajaid või kustutada olemasolevaid kasutajaid oma Azure Active Directory (Azure AD) ettevõtte kaudu.</span><span class="sxs-lookup"><span data-stu-id="06976-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="06976-130">Uue kasutaja lisamiseks logige [Azure ' i portaali](https://ms.portal.azure.com/#home) sisse organisatsiooni kasutaja administraatorina.</span><span class="sxs-lookup"><span data-stu-id="06976-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="06976-131">Valige **Azure Active Directory**, valige **Kasutajad** ja seejärel klõpsake nuppu **Uus kasutaja**.</span><span class="sxs-lookup"><span data-stu-id="06976-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="06976-132">Täitke lehel **kasutaja** nõutavad andmed.</span><span class="sxs-lookup"><span data-stu-id="06976-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="06976-133">Klõpsake nuppu **Loo**.</span><span class="sxs-lookup"><span data-stu-id="06976-133">Click **Create**.</span></span> <span data-ttu-id="06976-134">Kasutaja on loodud ja lisatud teie Azure AD rentniku jaoks.</span><span class="sxs-lookup"><span data-stu-id="06976-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="06976-135">**Lisateavet leiate** järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="06976-135">**Learn more**:</span></span>

- [<span data-ttu-id="06976-136">Uue kasutaja lisamine</span><span class="sxs-lookup"><span data-stu-id="06976-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="06976-137">Kasutaja kustutamine</span><span class="sxs-lookup"><span data-stu-id="06976-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="06976-138">Kasutaja profiili teabe lisamine või värskendamine Azure Active Directory abil</span><span class="sxs-lookup"><span data-stu-id="06976-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="06976-139">**Soovitatavad dokumendid**</span><span class="sxs-lookup"><span data-stu-id="06976-139">**Recommended documents**</span></span>

- [<span data-ttu-id="06976-140">Mis on roll-Based Access Control (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="06976-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="06976-141">Azure ' i eri rollide mõistmine</span><span class="sxs-lookup"><span data-stu-id="06976-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="06976-142">Administraatori rolli õigused Azure Active Directorys</span><span class="sxs-lookup"><span data-stu-id="06976-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="06976-143">Õpetus: kasutajale RBAC ja Azure ' i portaali kaudu juurdepääsu andmine</span><span class="sxs-lookup"><span data-stu-id="06976-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="06976-144">Azure ' i RBAC tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="06976-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="06976-145">Ressursside korraldamine Azure ' i halduse rühmadega</span><span class="sxs-lookup"><span data-stu-id="06976-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="06976-146">Azure ' i arve koopia taotlemine meili teel</span><span class="sxs-lookup"><span data-stu-id="06976-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="06976-147">Azure ' i krediidi-või deebetkaardi lisamine, värskendamine või eemaldamine</span><span class="sxs-lookup"><span data-stu-id="06976-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="06976-148">Tellimuse haldamine (uuesti aktiveerimine/tühistamine/vahetamine)</span><span class="sxs-lookup"><span data-stu-id="06976-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



