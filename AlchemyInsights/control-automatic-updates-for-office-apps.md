---
title: Office ' i rakenduste automaatsete värskenduste reguleerimine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438994"
---
# <a name="control-automatic-updates-for-office-apps"></a>Office ' i rakenduste automaatsete värskenduste reguleerimine

Vaikimisi laaditakse Office ' i rakenduste värskendused automaatselt alla ja rakendatakse taustal ilma kasutaja sekkumiseta. Administraatorid saavad siiski määrata, kuidas värskendusi Office Update ' i sätete abil rakendada. Sätete värskendamine võimaldab administraatoritel lubada või keelata automaatvärskendused, kuvada või peita Office ' i nupp **Värskenda kohe** , määrata värskendamise tähtajad ja muud. Üksikasjalikku teavet leiate järgmistest teemadest:

- [Office ' i värskenduste sätete konfigureerimine](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Office ' i automaatne värskendamine pole lubatud](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Office ' i värskendamise määratlemine pärast selle installimist](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Klientarvutile rakendatud olemasolevate värskenduste sätete vaatamiseks tehke järgmist.

1. Avage registriredaktor, minnes käsule **Start**  >  **Käivita**  >  **regedit**.
2. Aktiveerige järgmine asukoht ja vaadake üle Office ' i värskendamise sätted.  
    loomine. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Märkus**  Kui OfficeMgmtCOM võti on seatud, võidakse kuvada **Office '** i  >  **konto**  >  **Office**' i värskenduste kaudu teade "värskendusi haldab teie süsteemiadministraator". Lisateavet leiate teemast Microsoft [365 rakenduste värskenduste haldamine Microsoft Endpoint Configuration Manageri abil](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  