---
title: Organisatsioonisuhte loomine, et kasutajad saavad teha koostööd mõne muu asutusega
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816124"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="47afa-102">Organisatsioonisuhte loomine, et kasutajad saavad teha koostööd mõne muu asutusega</span><span class="sxs-lookup"><span data-stu-id="47afa-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="47afa-103">Avage Microsoft 365 halduskeskuse armatuurlaual Admin   >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="47afa-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="47afa-104">Avage ettevõtte  >  **ühiskasutus**.</span><span class="sxs-lookup"><span data-stu-id="47afa-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="47afa-105">Klõpsake **jaotises Ettevõtte ühiskasutus** nuppu **Uus** .</span><span class="sxs-lookup"><span data-stu-id="47afa-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="47afa-106">Tippige **uue organisatsioonisuhte** väljale **Seose** nimi organisatsioonisuhte sõbralik nimi.</span><span class="sxs-lookup"><span data-stu-id="47afa-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="47afa-107">Tippige **väljale Domains to share with** (Domeenid, mida soovite ühiskasutusse anda) selle välise Office 365 või Exchange'i asutuse domeeni, kus soovite oma kalendreid vaadata.</span><span class="sxs-lookup"><span data-stu-id="47afa-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="47afa-108">Kui teil on vaja sisestada mitu domeeni, eraldage domeeninimed komaga.</span><span class="sxs-lookup"><span data-stu-id="47afa-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="47afa-109">Näiteks contoso.com service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="47afa-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="47afa-110">Märkige ruut **Luba kalendri vaba/hõivatud aja teabe ühiskasutus,** et lülitada kalendri ühiskasutus sisse teie loetletud domeenidega.</span><span class="sxs-lookup"><span data-stu-id="47afa-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="47afa-111">Määrake kalendri vaba/hõivatud aja teabe ühiskasutustase ja määrake, millised kasutajad saavad kalendri vaba/hõivatud aja teavet ühiskasutusse anda.</span><span class="sxs-lookup"><span data-stu-id="47afa-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="47afa-112">Vaba/hõivatud juurdepääsu taseme miseks valige üks järgmistest.</span><span class="sxs-lookup"><span data-stu-id="47afa-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="47afa-113">**Kalendri vaba/hõivatud aja teave ainult ajaga**</span><span class="sxs-lookup"><span data-stu-id="47afa-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="47afa-114">**Kalendri vaba/hõivatud aja, teema ja asukohaga**</span><span class="sxs-lookup"><span data-stu-id="47afa-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="47afa-115">Kui soovite määrata, millised kasutajad kalendri vaba/hõivatud aja teavet jagavad, valige üks järgmistest.</span><span class="sxs-lookup"><span data-stu-id="47afa-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="47afa-116">**Kõik teie asutuse administraatorid**</span><span class="sxs-lookup"><span data-stu-id="47afa-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="47afa-117">**Määratud turberühm**</span><span class="sxs-lookup"><span data-stu-id="47afa-117">**A specified security group**</span></span>  

<span data-ttu-id="47afa-118">Klõpsake **loendis** turberühma valimiseks nuppu Sirvi ja seejärel klõpsake **nuppu ok**.</span><span class="sxs-lookup"><span data-stu-id="47afa-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="47afa-119">Klõpsake **organisatsioonisuhte** loomiseks nuppu Salvesta.</span><span class="sxs-lookup"><span data-stu-id="47afa-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="47afa-120">**Märkus.** Rentnikuülesed konfiguratsioonid ei toeta vaba/hõivatud otsingu jaoks isiklikke kontakte.</span><span class="sxs-lookup"><span data-stu-id="47afa-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="47afa-121">Vaba/hõivatud otsingu tööks tuleb kontaktid kaasata globaalsesse aadressiloendisse.</span><span class="sxs-lookup"><span data-stu-id="47afa-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="47afa-122">**Selle teema täielikuks mõistmiseks lugege:**</span><span class="sxs-lookup"><span data-stu-id="47afa-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="47afa-123">Organisatsioonisuhte loomine Exchange Online'is</span><span class="sxs-lookup"><span data-stu-id="47afa-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="47afa-124">Organisatsioonisuhte muutmine Exchange Online'is</span><span class="sxs-lookup"><span data-stu-id="47afa-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="47afa-125">Organisatsioonisuhte eemaldamine Exchange Online'is</span><span class="sxs-lookup"><span data-stu-id="47afa-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
