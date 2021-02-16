---
title: Rühmapoliitika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256714"
---
# <a name="group-policy"></a><span data-ttu-id="e7aaa-102">Rühmapoliitika</span><span class="sxs-lookup"><span data-stu-id="e7aaa-102">Group policy</span></span>

<span data-ttu-id="e7aaa-103">Azure Active Directory Domain Services (Azure AD DS) kasutajate ja arvuti objektide sätteid hallatakse sageli rühmapoliitika objektide (GPO) abil.</span><span class="sxs-lookup"><span data-stu-id="e7aaa-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="e7aaa-104">Azure AD DS sisaldab sisseehitatud lubatu AADDC kasutajate ja AADDC arvutite jaoks.</span><span class="sxs-lookup"><span data-stu-id="e7aaa-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="e7aaa-105">Teie keskkonna jaoks vajaliku rühmapoliitika konfigureerimiseks saate kohandada neid sisseehitatud lubatu.</span><span class="sxs-lookup"><span data-stu-id="e7aaa-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="e7aaa-106">Azure AD DC administraatorite rühma liikmetel on Azure AD DS-i domeenis rühmapoliitika halduse privileegid ning saate luua ka kohandatud GPO-d ja korralduslikke üksusi.</span><span class="sxs-lookup"><span data-stu-id="e7aaa-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="e7aaa-107">Lisateavet rühmapoliitika ja selle töötamise kohta leiate teemast [rühmapoliitika ülevaade](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="e7aaa-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="e7aaa-108">Hübriid-keskkonnas ei sünkroonita kohapealses AD DS-keskkonnas konfigureeritud rühmapoliitika Azure AD DS-iga.</span><span class="sxs-lookup"><span data-stu-id="e7aaa-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="e7aaa-109">Azure AD DS-is kasutajate või arvutite jaoks konfiguratsiooniseadete määratlemiseks redigeerige mõnda vaike-lubatu või looge kohandatud GPO.</span><span class="sxs-lookup"><span data-stu-id="e7aaa-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="e7aaa-110">See artikkel [rühmapoliitika haldamine](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) näitab teile, kuidas installida rühmapoliitika juhtimise vahendeid, kuidas ton redigeerida sisseehitatud lubatu ja kuidas luua kohandatud lubatu.</span><span class="sxs-lookup"><span data-stu-id="e7aaa-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



