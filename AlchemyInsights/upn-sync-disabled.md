---
title: UPN-i sünkroonimine on keelatud
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749510"
---
# <a name="upn-sync-disabled"></a>UPN-i sünkroonimine on keelatud

Kui alustasite Azure AD-ga sünkroonimist enne 30. märtsi 2016, käivitage järgmine Azure AD PowerShelli cmdlet-käsk, et lubada ainult teie asutuse UPN Soft Match.
  
 **Set-MsolDirSyncFeature-funktsioon EnableSoftMatchOnUpn-Enable $True**
  
UPN Soft Match lülitatakse automaatselt sisse organisatsioonidele, mis hakkasid Azure AD-ga sünkroonima 30. märtsi 2016.
  
Lisateavet UPN-i ja muude sünkroonimise funktsioonide sujuva vaste lubamise kohta leiate teemast [AZURE ad Connecti sünkroonimise teenuste funktsioonid](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

