---
title: Outlookis lisandmoodulite lisamise ajal on mitu kasutajat Accessi tõrgetega keelatud
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423717"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="56ca6-102">Outlookis lisandmoodulite lisamise ajal on mitu kasutajat Accessi tõrgetega keelatud</span><span class="sxs-lookup"><span data-stu-id="56ca6-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="56ca6-103">Saate määrata, millised teie asutuse administraatorid omavad Outlooki lisandmoodulite installimise ja haldamise õigust.</span><span class="sxs-lookup"><span data-stu-id="56ca6-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="56ca6-104">Samuti saate määrata, millistel ettevõtte kasutajatel on õigus lisandmooduleid oma tarbeks installida ja hallata.</span><span class="sxs-lookup"><span data-stu-id="56ca6-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="56ca6-105">Lisateavet leiate teemast [administraatorite ja kasutajate määramine, kes saavad Outlooki lisandmooduleid installida ja hallata](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="56ca6-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="56ca6-106">Kui soovite kinnitada, et olete kasutaja jaoks kasutajale õiguse määranud, asendage selle <Role Name> rolli nimi, mida soovite kontrollida, ja käivitage järgmine käsk Exchange Online PowerShellis.</span><span class="sxs-lookup"><span data-stu-id="56ca6-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="56ca6-107">Get-ManagementRoleAssignment-roll " <Role Name> "-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="56ca6-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="56ca6-108">Selles näites kirjeldatakse, kuidas kinnitada, kellele olete Office ' i poest Office ' i poest lisandmoodulite installimise õiguse määranud.</span><span class="sxs-lookup"><span data-stu-id="56ca6-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="56ca6-109">PowerShelli</span><span class="sxs-lookup"><span data-stu-id="56ca6-109">PowerShell</span></span>

<span data-ttu-id="56ca6-110">-Roll "org turuplatsi rakendused"-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="56ca6-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="56ca6-111">Tulemite ManagementRoleAssignment saate vaadata veerus tõhus kasutajad olevaid kandeid.</span><span class="sxs-lookup"><span data-stu-id="56ca6-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="56ca6-112">Üksikasjalikku teavet süntaksi ja parameetrite kohta leiate teemast [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="56ca6-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 