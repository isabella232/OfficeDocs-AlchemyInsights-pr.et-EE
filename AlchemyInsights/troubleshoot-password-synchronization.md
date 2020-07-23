---
title: Parooli sünkroonimise tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387873"
---
# <a name="troubleshoot-password-synchronization"></a>Parooli sünkroonimise tõrkeotsing

Parooli sünkroonimise probleemide tõrkeotsingu ks alustage selle AAD connect i tõrkeotsingu toimingu abil, et teha kindlaks, miks paroolid ei sünkroonita. Alustamiseks [halda otsesünkroonimist](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Avage uus Windows PowerShelli seanss oma Azure AD Ühenduse serveris ja valige suvand **Käivita administraatorina** .

2. Käivitage Set-ExecutionPolicy RemoteSigned või Set-ExecutionPolicy piiranguteta.

3. Käivitage Azure AD ühenduse viisard.

4. lehele Täiendavad tööülesanded > **Järgmine tõrkeotsing**  >  **Next**.

5. PowerShelli tõrkeotsingumenüü avamiseks valige **Käivita.**

6. Valige **Parooli sünkroonimise tõrkeotsing**.

    Probleem on tavaliselt selles, et parooli ei sünkroonita kindla kasutajakonto jaoks.

    **Märkmed** Parooli sünkroonimine nurjub, kui viimane edukas parooli sünkroonimine oli mõni aeg tagasi.

Lisateavet parooli sünkroonimise tõrkeotsingu kohta leiate teemast [Parooli räsisünkroonimise tõrkeotsing Azure AD Connecti sünkroonimisega](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).