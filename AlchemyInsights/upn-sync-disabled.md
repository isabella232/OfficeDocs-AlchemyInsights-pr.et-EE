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
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532327"
---
# <a name="upn-sync-disabled"></a>UPN sync puudega

Kui enne 30. märts 2016, Azure AD sünkroonimine käivitage järgmine Azure AD PowerShelli cmdlet-käsk et UPN pehme mängu ainult oma organisatsiooni:
  
 **Set-MsolDirSyncFeature-on EnableSoftMatchOnUpn-lubade kasutada $True programmi**
  
UPN pehme mängu lülitatakse automaatselt organisatsioonidele, kes hakkas Azure AD või hiljem 30 märts 2016 sünkroonimist.
  
Mis võimaldab pehme mängu UPN ja muid sünkroonimise kohta lisateabe saamiseks lugege [Azure AD ühenduse sünkroonimise teenuse funktsioone](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

