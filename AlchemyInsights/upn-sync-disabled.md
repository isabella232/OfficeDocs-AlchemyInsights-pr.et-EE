---
title: UPN-i sünkroonimine on keelatud
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726100"
---
# <a name="upn-sync-disabled"></a>UPN-i sünkroonimine on keelatud

Kui käivitate sünkroonimise Azure AD enne 30 märts 2016, käivitage järgmine Azure AD PowerShelli cmdlet-käsu lubamiseks UPN pehme vaste oma organisatsiooni ainult:
  
 **Set-MsolDirSyncFeature-funktsioon EnableSoftMatchOnUpn-luba $True**
  
UPN pehme vaste on automaatselt sisse lülitatud organisatsioonidele, mis hakkasid sünkroonimise Azure AD või pärast 30 märts 2016.
  
Lisateabe saamiseks lubamine pehme vaste UPN ja muud sünkroonimise funktsioone, vaadake [AZURE AD ühenduse sünkroonimise teenuse funktsioone](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

