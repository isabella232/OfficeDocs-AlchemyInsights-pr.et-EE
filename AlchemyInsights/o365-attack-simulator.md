---
title: 2681 Attack Simulator Microsoft 365
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
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801547"
---
# <a name="attack-simulator-in-microsoft-365"></a>Rünnaku simulaator Microsoft 365

- Kas teil on puudu rünnaku simulaator? Attack Simulator nõuab **Microsoft Defender office 365 leping 2 (ATP leping 2)** või **Office 365 Enterprise E5** . Rakenduses Microsoft Defender for Office 365 leping 1 (ATP leping 1), Office 365 Enterprise E3 või Microsoft 365 ettevõtetele mõeldud Office ' i pakettide jaoks **ei ole** rünnaku simulaatorit kaasatud.

- Simuleeritud rünnakute käivitamiseks kasutatav konto peab olema üldadministraator või administraatori õigused ja mitme teguriga autentimine (MFA). Lisateavet rünnaku simulaatori nõuete kohta leiate [sellest teemast](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Tähtsamaid asju teada **Brute Force Password** Attack simulatsioonid:

  - Kui TARGETi kontol on MFA lubatud ja parool on õigesti kajastatud, ei kuvata kontot ohustatud kujul (teine autentimine on puudulik).

  - Parool ei tohi olla suurem kui 10 MB. Kasutage ühte parooli rea kohta ja lisage loendi viimasele paroolile tühi rida (veo tagastus).

- Olulised asjad, mida saab teada **oda andmepüügiga** seotud simulatsioonide kohta.

  - Kujunduse järgi ei saa te **andmepüügi sisselogimise serveri URL-i** jaoks kohandatud väärtust anda.

  - Kui adressaat kasutab teate saatmiseks [lisandmoodulit luba](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) sõnum andmepüügiks, siis ei pruugi te saada sõnumile teatisi (kuna tegemist on simuleeritud rünnakuga).

- Aruanded: pärast simuleeritud rünnaku lõpulejõudmist võite aruande kuvamiseks klõpsata nuppu **rünnaku üksikasjad** .

- Üksikasjalikud juhised ja uued funktsioonid rakenduses Attack Simulator leiate teemast [rünnaku simulaator Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
