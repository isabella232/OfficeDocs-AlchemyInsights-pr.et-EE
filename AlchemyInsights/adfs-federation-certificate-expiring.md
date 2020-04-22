---
title: ADFS Föderatsiooni serdi aegumine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710403"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Föderatsiooni serdi aegumine

Selle probleemi lahendamiseks toimige järgmiselt.
  
1. Installige Microsoft Azure Active Directory moodul Windows PowerShell arvutis (kui moodul pole juba installitud). Selleks [hallata AZURE ad Windows PowerShelli abil](https://aka.ms/aadposh).

2. Järgige juhiseid "stsenaarium 1: AD FS luba allkirjastamise sert on aegunud" jaotises ["ilmnes probleem saidile" AD FS kui välise kasutaja logib sisse Microsoft 365, Azure või Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Järgige juhiseid [värskendada või parandada välise domeeni Microsoft, Azure või Intune sätteid](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Föderatsiooni sertide uuendamise kohta lisateabe saamiseks vaadake [uuendada Föderatsiooni serdid Microsoft 365 ja Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
