---
title: UPN sync puudega
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286118"
---
# <a name="upn-sync-disabled"></a>UPN sync puudega

Kui enne 30. märts 2016, Azure AD sünkroonimine käivitage järgmine Azure AD PowerShelli cmdlet-käsk et UPN pehme mängu ainult oma organisatsiooni:
  
 **Set-MsolDirSyncFeature-on EnableSoftMatchOnUpn-lubade kasutada $True programmi**
  
UPN pehme mängu lülitatakse automaatselt organisatsioonidele, kes hakkas Azure AD või hiljem 30 märts 2016 sünkroonimist.
  
Mis võimaldab pehme mängu UPN ja muid sünkroonimise kohta lisateabe saamiseks lugege [Azure AD ühenduse sünkroonimise teenuse funktsioone](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

