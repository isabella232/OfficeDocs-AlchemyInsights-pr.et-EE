---
title: Paroolisünkroonimise tõrkeotsing
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
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105744"
---
# <a name="troubleshoot-password-synchronization"></a>Paroolisünkroonimise tõrkeotsing

Paroolisünkroonimisprobleemide tõrkeotsinguks käivitage see AAD-Ühendus, et teha kindlaks, miks paroole ei sünkroonita. Alustamiseks avage [Otsesünkroonimise haldamine](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Avage azure Windows PowerShell AD Ühendus uus seanss ja valige suvand **Käivita administraatorina.**

2. Käivitage Set-ExecutionPolicy RemoteSigned või Set-ExecutionPolicy Piiranguteta.

3. Käivitage Azure AD Ühendus viisard.

4. Avage leht Lisaülesanded ja > **Tõrkeotsing**  >  **järgmine**.

5. **PowerShelli** tõrkeotsingumenüü avamiseks valige Käivita.

6. Valige **Tõrkeotsing paroolisünkroonimiseks**.

    Tavaliselt on probleem selles, et teatud kasutajakonto parooli ei sünkroonita.

    **Märkmed** Parooli sünkroonimine nurjub, kui viimane parooli sünkroonimine õnnestus mõni aeg tagasi.

Lisateavet paroolisünkroonimise tõrkeotsingu kohta leiate teemast [Paroolisiga sünkroonimise tõrkeotsing Azure AD Ühendus sünkroonimisega.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)