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
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921704"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="ac720-102">UPN sync puudega</span><span class="sxs-lookup"><span data-stu-id="ac720-102">UPN sync disabled</span></span>

<span data-ttu-id="ac720-103">Kui enne 30. märts 2016, Azure AD sünkroonimine käivitage järgmine Azure AD PowerShelli cmdlet-käsk et UPN pehme mängu ainult oma organisatsiooni:</span><span class="sxs-lookup"><span data-stu-id="ac720-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="ac720-104">**Set-MsolDirSyncFeature-on EnableSoftMatchOnUpn-lubade kasutada $True programmi**</span><span class="sxs-lookup"><span data-stu-id="ac720-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="ac720-105">UPN pehme mängu lülitatakse automaatselt organisatsioonidele, kes hakkas Azure AD või hiljem 30 märts 2016 sünkroonimist.</span><span class="sxs-lookup"><span data-stu-id="ac720-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="ac720-106">Mis võimaldab pehme mängu UPN ja muid sünkroonimise kohta lisateabe saamiseks lugege [Azure AD ühenduse sünkroonimise teenuse funktsioone](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="ac720-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

