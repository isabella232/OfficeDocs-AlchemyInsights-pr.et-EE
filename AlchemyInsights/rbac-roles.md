---
title: 'RBAC rollid '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583550"
---
# <a name="rbac-rules"></a><span data-ttu-id="19a17-102">RBAC reeglid</span><span class="sxs-lookup"><span data-stu-id="19a17-102">RBAC rules</span></span>

<span data-ttu-id="19a17-103">Kui teil on õigus viga, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="19a17-103">If you get the permission error:</span></span> 

- <span data-ttu-id="19a17-104">**Kliendil, kellel on objekti ID, ei ole lubatud ulatuses toiminguid teha (kood: AuthorizationFailed)**: kui proovite luua ressurssi, siis kontrollige, kas olete praegu sisse logitud kasutajaga, kellele on määratud roll, millel on valitud ulatuses ressursile kirjutamise õigus.</span><span class="sxs-lookup"><span data-stu-id="19a17-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="19a17-105">Kui soovite näiteks hallata virtuaalseid masinaid ressursirühma, peaks teil olema ressursi rühmas (või vanemas ulatuses) [virtuaalarvuti kaastööline](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) roll.</span><span class="sxs-lookup"><span data-stu-id="19a17-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="19a17-106">Iga sisseehitatud rolli kasutusõiguste loendi leiate teemast [Azure ' i ressursside sisseehitatud rollid](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="19a17-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="19a17-107">**Teil pole tugiteenuste taotluse loomise õigust**: kui proovite luua või värskendada tugiteenuse piletit, siis kontrollige, kas olete praegu sisse logitud kasutajaga, kellele on määratud Microsoft. support/supportTickets/Write õigus (nt [tugiteenuste taotluse kaastööd](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)).</span><span class="sxs-lookup"><span data-stu-id="19a17-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="19a17-108">Rolli **ei saa enam määrata (kood: RoleAssignmentLimitExceeded)**: kui proovite rolli määrata, püüdke vähendada rollimäärangu arvu, määrates selle asemel rollid rühmadesse.</span><span class="sxs-lookup"><span data-stu-id="19a17-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="19a17-109">Azure toetab kuni **2000** rolli määramist tellimuse kohta.</span><span class="sxs-lookup"><span data-stu-id="19a17-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="19a17-110">Azure ' i RBAC rollide kohta leiate lisateavet teemast [Azure ' i RBAC rollid](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="19a17-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
