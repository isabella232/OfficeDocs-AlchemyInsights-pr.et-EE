---
title: Üksik kasutaja ei näe outlooki lisandmooduleid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197833"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="86dd2-102">Üksik kasutaja ei näe outlooki lisandmooduleid</span><span class="sxs-lookup"><span data-stu-id="86dd2-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="86dd2-103">Kasutaja võib olla osa rollist, millel pole õiget parameetrit AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="86dd2-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="86dd2-104">Käivitage see cmdlet-käsk, et teada saada, kas kasutajaga on seotud õige roll:</span><span class="sxs-lookup"><span data-stu-id="86dd2-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="86dd2-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -$false delegeerimine | Vormindus-tabel -Auto Roll,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="86dd2-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="86dd2-106">Lisateavet leiate teemast [Outlooki lisandmoodulite installimiseks ja haldamiseks administraatorite ja kasutajate määramine](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="86dd2-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
