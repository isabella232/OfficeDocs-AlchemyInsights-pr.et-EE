---
title: Teisalda e-kirjad arhiivi postkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713642"
---
# <a name="move-email-to-the-archive-mailbox"></a>Teisalda e-posti arhiivi postkasti

1. Veenduge, et **arhiivi postkast** on lubatud. Kui ei, kasutage [selle artikli](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) juhiseid arhiivi postkasti lubamiseks.

2. Sõnumite automaatseks arhiivimiseks arhiivi postkasti, tuleb seada säilitamise silt koos **Teisalda arhiivi** toiming **automaatselt rakendada kogu postkasti (vaikimisi) silt**. Sildi loomiseks kasutage siin olevaid juhiseid: [Arhiiv vaikimisi silt](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Järgmisena lisage oma säilituspoliitikale **arhiivi** silt. Exchange ' i halduskeskus, valige **säilituspoliitikad** > lisa **Arhiiv arhiivi sildi** poliitika > **salvestada**.

4. Nüüd [määrata säilituspoliitika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkreetse kasutaja postkasti. Sama poliitika rakendatakse nii **põhi** -kui ka **arhiivi** postkasti.

Võib osutuda vajalikuks sundida hallatav kaustade abimees (MFA) käivitada ja rakendada uusi sätteid kasutaja postkasti. Käivitage järgmine käsk [ühendatud EXO PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) käivitada hallatav kaust Assistant konkreetse postkasti:
  
Start-ManagedFolderAssistant-identiteet<name of the mailbox>

Lisateavet arhiivipoliitika seadistamise kohta leiate jaotisest [arhiivi-ja kustutuspoliitika häälestamine postkastide jaoks](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  