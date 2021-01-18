---
title: Rühmade määramine Azure AD rollile
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884914"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="f3170-102">Rühmade määramine Azure AD rollile</span><span class="sxs-lookup"><span data-stu-id="f3170-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="f3170-103">Azure AD rühma määramiseks, kus on Azure AD ' i asutuse allikas Azure AD rollis, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="f3170-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="f3170-104">Uue rühma loomine – uue rühma loomiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="f3170-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="f3170-105">loomine.</span><span class="sxs-lookup"><span data-stu-id="f3170-105">a.</span></span> <span data-ttu-id="f3170-106">Logige sisse Azure AD halduskeskus, millel on **priviligeeritud rollide administraator** või **üldadministraatori** õigused.</span><span class="sxs-lookup"><span data-stu-id="f3170-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="f3170-107">b.</span><span class="sxs-lookup"><span data-stu-id="f3170-107">b.</span></span> <span data-ttu-id="f3170-108">Valige **Azure Active Directory > rühmad > kõik rühmad > uus rühm**.</span><span class="sxs-lookup"><span data-stu-id="f3170-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="f3170-109">c.</span><span class="sxs-lookup"><span data-stu-id="f3170-109">c.</span></span> <span data-ttu-id="f3170-110">Looge rühm.</span><span class="sxs-lookup"><span data-stu-id="f3170-110">Create the group.</span></span>

2. <span data-ttu-id="f3170-111">Määrake rühmale roll rühma loomise ajal või pärast rühma loomist.</span><span class="sxs-lookup"><span data-stu-id="f3170-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="f3170-112">loomine.</span><span class="sxs-lookup"><span data-stu-id="f3170-112">a.</span></span> <span data-ttu-id="f3170-113">Rühmale rolli määramiseks rühma loomise ajal lülitage sisse lüliti **AZURE ad rollid** , mida saab rühmale määrata ja rühma luua.</span><span class="sxs-lookup"><span data-stu-id="f3170-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="f3170-114">b.</span><span class="sxs-lookup"><span data-stu-id="f3170-114">b.</span></span> <span data-ttu-id="f3170-115">Kui soovite rühmale rolli määrata pärast selle loomist, liikuge vastloodud rühma jaoks menüüsse **määratud rollid** ja määrake roll rühmale.</span><span class="sxs-lookup"><span data-stu-id="f3170-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="f3170-116">**Azure AD rollile määratud rühma liikmelisuse haldamine**</span><span class="sxs-lookup"><span data-stu-id="f3170-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="f3170-117">Õiguste suurendamise vältimiseks saab vaikimisi kasutada ainult privilegeeritud rolli administraatorid ja globaalsed administraatorid rollile määratud rühma liikmestaatust.</span><span class="sxs-lookup"><span data-stu-id="f3170-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="f3170-118">Nad saavad siiski määrata sellise rühma omaniku ja selle ülesande delegeerida.</span><span class="sxs-lookup"><span data-stu-id="f3170-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="f3170-119">Lisateavet pilve rühmade Azure AD rollide määramise kohta leiate teemast [ad rollide määramine pilve rühmale](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="f3170-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="f3170-120">Lisateavet pilveteenuste jaoks määratud rollide tõrkeotsingu kohta leiate teemast [pilve rühmade jaoks määratud rollide tõrkeotsing](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="f3170-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





