---
title: Intune ' i administraatori konsooli kasutamise probleemid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555037"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="2889c-102">Intune ' i administraatori konsooli kasutamise probleemid</span><span class="sxs-lookup"><span data-stu-id="2889c-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="2889c-103">**Intune ' i administraatori portaali navigeerimisel "juurdepääs keelatud".**</span><span class="sxs-lookup"><span data-stu-id="2889c-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="2889c-104">Kui olete kohandatud rolli Intune ' i liige, veenduge, et teie kontole on määratud Intune ' i või Enterprise Mobility Suite (EMS) litsents.</span><span class="sxs-lookup"><span data-stu-id="2889c-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="2889c-105">Kui kasutate seadmete haldamiseks Configuration Manageri, siis veenduge, et te ei kuuluks Configuration Manageri MDM-i kasutaja kollektsiooni Intune ' i.</span><span class="sxs-lookup"><span data-stu-id="2889c-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="2889c-106">Veenduge, et teile on määratud roll-põhine halduse kontrolli (RBAC) load Intune rollid Blade.</span><span class="sxs-lookup"><span data-stu-id="2889c-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="2889c-107">Veenduge, et kasutatav rühm pole leviloend.</span><span class="sxs-lookup"><span data-stu-id="2889c-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="2889c-108">Azure ' i portaalis saab Intune ' i ainult toetada kasutajakontosid, mis kuuluvad Azure Active Directory turbe rühmadesse.</span><span class="sxs-lookup"><span data-stu-id="2889c-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="2889c-109">Vaadake üle oma rühmad Azure ' i portaalis > **Intune**' i  >  **rühmad**või Azure ' i portaalis > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="2889c-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="2889c-110">**Kasutajal on määratud Intune ' i rolli jaoks liiga palju õiguseid**</span><span class="sxs-lookup"><span data-stu-id="2889c-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="2889c-111">Soovitage kasutajal minna Intune Intune **Intune**  >  **Rollidele**, mida  >  **minu load**  >  **ekspordivad** antud õigustega tutvumiseks.</span><span class="sxs-lookup"><span data-stu-id="2889c-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="2889c-112">**Lisasin rollile rühma ulatuse, kuid selle rolli kasutajad näevad endiselt teisi kasutajaid või seadmeid.**</span><span class="sxs-lookup"><span data-stu-id="2889c-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="2889c-113">Rakendusala rühmad ei Filtreeri kasutajaid ega seadmeid.</span><span class="sxs-lookup"><span data-stu-id="2889c-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="2889c-114">Rakendusala rühmad:</span><span class="sxs-lookup"><span data-stu-id="2889c-114">Scope groups:</span></span>

- <span data-ttu-id="2889c-115">Saate piirata, kellele kasutajad saavad poliitikaid või rakendusi määrata.</span><span class="sxs-lookup"><span data-stu-id="2889c-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="2889c-116">Lubada ainult kindlatel kasutajatel kasutada seadmeid, mis ei tööta.</span><span class="sxs-lookup"><span data-stu-id="2889c-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="2889c-117">Lisateavet ulatuste rühmade kohta leiate artiklist [Role-Based Access Control (RBAC) Microsoft Intune ' is](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="2889c-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="2889c-118">**Lisasin kasutaja Intune rollile, kuid neil on endiselt täielik juurdepääs Intune konsoolile.**</span><span class="sxs-lookup"><span data-stu-id="2889c-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="2889c-119">Liikuge Azure ' i portaalis > **kasutajate** Intune ' i ja veenduge, et kasutaja poleks määratud Azure ' i portaalis ühelegi järgmistest rollidest.</span><span class="sxs-lookup"><span data-stu-id="2889c-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="2889c-120">Globaalne administraator</span><span class="sxs-lookup"><span data-stu-id="2889c-120">Global administrator</span></span>
- <span data-ttu-id="2889c-121">Teenuse administraatori Intune</span><span class="sxs-lookup"><span data-stu-id="2889c-121">Intune service administrator</span></span>
- <span data-ttu-id="2889c-122">SharePointi administraator</span><span class="sxs-lookup"><span data-stu-id="2889c-122">SharePoint administrator</span></span>

<span data-ttu-id="2889c-123">Lisateavet leiate artiklist [Role-Based Access Control (RBAC) Microsoft Intune ' is](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="2889c-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="2889c-124">**Accessi probleemid**</span><span class="sxs-lookup"><span data-stu-id="2889c-124">**Access Issues**</span></span>

<span data-ttu-id="2889c-125">Lisateavet leiate teemast [Office 365, Azure ' i või Intune ' i sisselogimine](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="2889c-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>