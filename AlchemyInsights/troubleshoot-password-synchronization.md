---
title: Parooli sünkroonimise tõrkeotsing
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664922"
---
# <a name="troubleshoot-password-synchronization"></a>Parooli sünkroonimise tõrkeotsing

Parooli sünkroonimise probleemide tõrkeotsinguks käivitage see AAD Connecti tõrkeotsing, et kindlaks teha, miks paroolid ei sünkroonita. Alustuseks valige [Halda otsest sünkroonimist](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Avage uus Windows PowerShelli seanss Azure AD Connecti serveris ja valige suvand **Käivita administraatorina** .

2. Run Set-ExecutionPolicy RemoteSigned või Set-ExecutionPolicy on piiramatud.

3. Käivitage Azure AD Connecti viisard.

4. Avage leht täiendavad tööülesanded > **tõrkeotsing**  >  **järgmiseks**.

5. Valige käsk **Käivita** , et avada menüü PowerShell tõrkeotsing.

6. Valige **parooli sünkroonimise tõrkeotsing**.

    Probleem on tavaliselt selles, et parooli ei sünkroonita kindla kasutajakonto jaoks.

    **Märkmed** Parooli sünkroonimine nurjub, kui viimase eduka parooli sünkroonimine oli mõni aeg tagasi.

Lisateavet parooli sünkroonimise tõrkeotsingu kohta leiate teemast [AZURE ad Connecti sünkroonimine parooliga Hash Synci tõrkeotsing](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).