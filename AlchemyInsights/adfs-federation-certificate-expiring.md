---
title: ADFS Federation Certificate Expiring
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952965"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation Certificate Expiring

Selle probleemi lahendamiseks tehke järgmist.
  
1. Installige Microsoft Azure Active Directory moodul Windows PowerShell (kui moodul pole veel installitud). Selleks avage Azure [AD haldamine](https://aka.ms/aadposh)Windows PowerShell.

2. Järgige AD FS-i tõrke "Ilmnes probleem saidile juurdepääsul" jaotises "Stsenaarium 1: AD FS-i loa allkirjastamise sert" toodud juhiseid, kui liitkasutaja [logib sisse rakendusse Microsoft 365, Azure või Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Täitke jaotises [Välisdomeeni sätete värskendamine või parandamine Microsoftis, Azure'is või Intune'is toodud juhised.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Lisateavet Föderatsiooni sertide uuendamise kohta leiate teemast Microsoft 365 ja [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
