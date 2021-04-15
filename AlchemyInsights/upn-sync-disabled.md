---
title: UPN-i sünkroonimine on keelatud
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782147"
---
# <a name="upn-sync-disabled"></a>UPN-i sünkroonimine on keelatud

Kui alustasite Azure AD-ga sünkroonimist enne 30. märtsi 2016, käivitage järgmine Azure AD PowerShelli cmdlet-käsk, et lubada UPN-i pehme vaste ainult teie ettevõtte jaoks.
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN-i pehme vaste on automaatselt sisse lülitatud nende ettevõtete jaoks, kes hakkasid Azure AD-ga sünkroonima 30. märtsil 2016 või hiljem.
  
Lisateavet UPN-i ja muude sünkroonimisfunktsiooni pehme vastete lubamise kohta leiate teemast [Azure AD Connecti sünkroonimisteenuse funktsioonid.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

