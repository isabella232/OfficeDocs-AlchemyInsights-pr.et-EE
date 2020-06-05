---
title: Probleemid sisselogimisel Microsoft 365 rakendused
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579933"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Microsoft 365 rakenduste parandamine "Vabandust, teine konto teie organisatsioonis on juba allkirjastatud" sõnum

Probleemi lahendamiseks proovige järgmist.

- Eemaldage kõik töökontod, välja arvatud mõjutatud konto, kasutades Windowsi sätteid > **juurdepääsu töö või kooli**.
- [Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , kasutades Windowsi mandaat Manager.<br/>
    **Märkus:** Office 2016 registri teed on muutunud 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Avage Office ' i rakendus, valige **faili**  >  **konto**  >  **Logi välja**. Seejärel logige sisse, kasutades kehtivat litsentsi kasutajakontoga. Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Maci kasutajad võiksid lugeda artiklit [Office 2016 for Maci rakendusse ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Lisateabe saamiseks vaadake ["Vabandust, teine konto teie organisatsioonis on juba sisse logitud selles arvutis" Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).