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
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511036"
---
# <a name="move-email-to-the-archive-mailbox"></a>Teisalda e-posti arhiivi postkasti

1. Veenduge, et **arhiivi postkast** on lubatud. Kui ei, kasutage [selle artikli](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) juhiseid arhiivi postkasti lubamiseks.

2. Sõnumite automaatseks arhiivimiseks arhiivi postkasti, tuleb seada säilitamise silt koos **Teisalda arhiivi** toiming **automaatselt rakendada kogu postkasti (vaikimisi) silt**. Sildi loomiseks kasutage siin olevaid juhiseid: [Arhiiv vaikimisi silt](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Järgmisena lisage oma säilituspoliitikale **arhiivi** silt. Exchange ' i halduskeskus, valige **säilituspoliitikad** > lisa **Arhiiv arhiivi sildi** poliitika > **salvestada**.

4. Nüüd [määrata säilituspoliitika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkreetse kasutaja postkasti. Sama poliitika rakendatakse nii **põhi** -kui ka **arhiivi** postkasti.

Võib osutuda vajalikuks sundida hallatav kaustade abimees (MFA) käivitada ja rakendada uusi sätteid kasutaja postkasti. Käivitage järgmine käsk [ühendatud EXO PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) käivitada hallatav kaust Assistant konkreetse postkasti:
  
Start-ManagedFolderAssistant-identiteet<name of the mailbox>

Lisateavet arhiivipoliitika seadistamise kohta leiate jaotisest [arhiivi-ja kustutuspoliitika häälestamine postkastide jaoks](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  