---
title: Tuvastada väline e-posti suunamine postkastid auditilogi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508948"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Tuvastada, kui väline e-posti suunamine on konfigureeritud postkastid

Kui Microsoft 365 kasutaja konfigureerib välise e-posti suunamine postkasti, tegevust auditeeritakse osana **Set-Mailbox cmdlet-** käsu. Tegevust saate vaadata auditilogi otsingu abil turbe-& Vastavuskeskuses.

1. Logige sisse [Microsoft 365 Security & vastavuse Center](https://protection.office.com/).

2. **otsingulehele otsingu**  >  **auditilogi** .

3. Saate **valida kuupäevavahemiku alguskuupäeva ja** **lõppkuupäeva** väljadel. Kasutajanime ei ole vaja määrata. Veenduge, et välja **Tegevused** väärtuseks kuvatakse **kõigi tegevuste tulemused**.

4. Klõpsake suvandit **Otsing**.

Tulemuste, klõpsake **filtri tulemused** ja tippige **määratud postkast** tegevuse filter kasti. Valige tulemite auditilogi. **Üksikasjade** hüpik, klõpsake **rohkem teavet**. Peate vaatama iga auditi kirje üksikasjad, et teha kindlaks, kas tegevus on seotud e-posti suunamine.

- **ObjectId**: muudetud postkasti alias väärtus.

- **Parameetrid**: _forwardingsmtpaddress_ näitab Target e-posti aadress.

- **Userid**: kasutaja, kes on konfigureeritud e-posti suunamine postkasti **ObjectId** välja.

Lisateabe saamiseks vaadake määrates, [kes seadistada e-posti suunamine postkasti](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
