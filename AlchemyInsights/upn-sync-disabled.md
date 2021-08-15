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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038108"
---
# <a name="upn-sync-disabled"></a>UPN-i sünkroonimine on keelatud

Kui alustasite Azure AD-ga sünkroonimist enne 30. märtsi 2016, käivitage järgmine Azure AD PowerShelli cmdlet-käsk, et lubada UPN-i pehme vaste ainult teie ettevõtte jaoks.
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN-i pehme vaste on automaatselt sisse lülitatud nende ettevõtete jaoks, kes hakkasid Azure AD-ga sünkroonima 30. märtsil 2016 või hiljem.
  
Lisateavet UPN-i ja muude sünkroonimisfunktsiooni pehme vastete lubamise kohta leiate teemast [Azure AD Ühendus sünkroonimisteenuse funktsioonid.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

