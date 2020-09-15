---
title: ADFS Föderatsiooni sert aegub
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686710"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Föderatsiooni sert aegub

Probleemi lahendamiseks tehke järgmist.
  
1. Installige Microsoft Azure Active Directory moodul Windows PowerShelli jaoks arvutis (kui moodul pole veel installitud). Selleks avage [Windows PowerShelli abil Azure ' i reklaami haldamine](https://aka.ms/aadposh).

2. Järgige juhiseid jaotises "stsenaarium 1: AD FS-i luba – allkirjastamise sert on aegunud" jaotisest " [tõrge juurdepääsul saidile" AD FS-i korral, kui väline kasutaja logib sisse Microsoft 365, Azure ' i või Intune ' i](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Järgige juhiseid [Microsoft, Azure ' i või Intune ' i ühendatud domeeni sätete värskendamise või parandamise](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)kohta.

    Lisateavet Föderatsiooni sertide uuendamise kohta leiate teemast [Microsoft 365 ja Azure Active Directory Föderatsiooni sertide pikendamine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
