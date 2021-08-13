---
title: Meilisõnumite teisaldamine arhiivipostkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974953"
---
# <a name="move-email-to-the-archive-mailbox"></a>Meilisõnumite teisaldamine arhiivipostkasti

Kui soovite, et käivitame allpool nimetatud sätete automaatse kontrollimise, valige selle lehe ülaosas < nupp Tagasi ja sisestage selle kasutaja meiliaadress, kellel on probleeme meilisõnumite arhiivipostkasti teisaldamisel.

1. Veenduge, et **arhiivipostkast** on lubatud. Kui ei, kasutage [arhiivipostkasti lubamiseks](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) selles artiklis toodud juhiseid.

2. Sõnumite automaatseks arhiivimiseks arhiivipostkasti tuleb  säilitussildiks, mille toiminguks on Teisalda arhiivimine, määrata kogu **postkastile (vaikesildile) automaatselt rakendatud.** Sildi loomiseks tehke järgmist. Vaikimisi sildi [arhiivimine](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Seejärel lisage **säilituspoliitikasse** silt Arhiiv. Valige Exchange halduskeskuses säilituspoliitikad **ja** > lisage  silt Teisalda arhiivi poliitikasse > **Salvesta**.

4. Nüüd [määrake säilituspoliitika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkreetse kasutaja postkastile. Sama poliitika rakendatakse nii esmasele **kui** ka **arhiivipostkastile.**

Võimalik, et on vaja sundida hallatava kausta abimeest (MFA) käivitama ja kasutaja postkastile uusi sätteid rakendama. Kindla postkasti hallatava kausta [abimehe käivitamiseks käivitage EXO PowerShelliga](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) ühendatud ajal järgmine käsk.
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Lisateavet arhiivipoliitika häälestamise kohta leiate teemast [Postkastide arhiivimis- ja kustutuspoliitika seadistamine.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  