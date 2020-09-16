---
title: Teamsi ülemineku edasilükkamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741767"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Microsoft orienteeritud Teamsi versiooni edasi lükkamine

**Oluline**: selle probleemi lahendamiseks saate kasutada tugiteenuste diagnostikat, kuid tundub, et te ei kasuta uut administreerimiskeskuset. Uue administreerimiskeskuse kasutamiseks libistage paremas ülanurgas olevale ülemisele paremale, mis ütleb, et **Uus halduskeskus** asub paremal. Kui kasutate uut Administreerimiskeskuset, klõpsake nuppu **Vajad abi?** vidinat, tippige käsk "töörühma uuendamine edasi" ja seejärel järgige diagnostika käivitamiseks viipasid.

Kui saite teate Microsofti juhitud automatiseeritud ülemineku kohta Skype ' i ärirakendusest Microsoft Teamsi ja te soovite automaatse ülemineku hilisemale kuupäevale edasi lükata, saab üldadministraator sisse logida [teamsi administraatori portaali](https://admin.teams.microsoft.com/dashboard) ja pärast nupu **Värskenda olekut** klõpsamist jaotises Microsoft teamsi täiendus valida nupp **Lükka edasi** . Kui soovite vaadata oma rentniku automaatse ülemineku uut kuupäeva Microsoft Teamsi, värskendage Teamsi administraatori portaali lehte.

**Märkus:** Nupp **Lükka edasi** on saadaval ainult juhul, kui olete saanud sõnumikeskuse teatise automatiseeritud versiooni kohta. 

Globaalsed administraatorid saavad kasutada ka [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) , et saada lisateavet nende praeguse täienduse oleku kohta.
