---
title: UPN sync puudega
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767222"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="db0e4-102">UPN sync puudega</span><span class="sxs-lookup"><span data-stu-id="db0e4-102">UPN sync disabled</span></span>

<span data-ttu-id="db0e4-103">Kui enne 30. märts 2016, Azure AD sünkroonimine käivitage järgmine Azure AD PowerShelli cmdlet-käsk et UPN pehme mängu ainult oma organisatsiooni:</span><span class="sxs-lookup"><span data-stu-id="db0e4-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="db0e4-104">**Set-MsolDirSyncFeature-on EnableSoftMatchOnUpn-lubade kasutada $True programmi**</span><span class="sxs-lookup"><span data-stu-id="db0e4-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="db0e4-105">UPN pehme mängu lülitatakse automaatselt organisatsioonidele, kes hakkas Azure AD või hiljem 30 märts 2016 sünkroonimist.</span><span class="sxs-lookup"><span data-stu-id="db0e4-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="db0e4-106">Mis võimaldab pehme mängu UPN ja muid sünkroonimise kohta lisateabe saamiseks lugege [Azure AD ühenduse sünkroonimise teenuse funktsioone](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="db0e4-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

