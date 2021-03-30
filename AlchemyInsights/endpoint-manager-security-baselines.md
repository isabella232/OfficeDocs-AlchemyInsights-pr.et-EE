---
title: EndPoint Manager – turbealused
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420877"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – turbealused

Turbealused on windowsi sätete eel konfigureeritud rühmad, mis aitavad teil rakendada vastavate turberühmade soovitatud turbesätteid. Neid alusjooni saab kohandada nii, et need edastaks ainult soovitud sätted ja väärtused. Lisateavet turbe alusjoonte kohta leiate teemast Windows 10 seadmete konfigureerimine [Intune'i turbe alusjoonte abil.](https://docs.microsoft.com/mem/intune/protect/security-baselines)

Praegu on nende toodete jaoks alusjooned.

- Windowsi MDM-i turbesätted
- Microsoft Defender endPointi turbe jaoks
- Microsoft Edge

Kõiki lähtejooni värskendatakse perioodiliselt ja need akrementversioonides. Iga versioon lisab ja eemaldab eelmise versiooni sätted, et veenduda, et alusjoon vastab praegustele juhistele. Lõpp-punkti turbe turbe võrdluskonsool võimaldab võrrelda erinevaid versioone, muutes muudatused versioonist versiooniks nähtavaks.

Juhised selle kohta, kuidas lähtejoone versiooni kõige tõhusamalt muuta, leiate teemast [Microsoft Intune'i turbe alusprofiilide haldamine.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

Pärast turbetaseme juurutamist saate juurutamise olekut jälgida ja sätteid seadme kaupa üle vaadata.

**Märkus.** Lähteandmete aruandluseks võib võtta kuni 24 tundi alates algsest juurutamisest kuni seadmeni ja kuni 6 tundi täiendavate värskenduste saamiseks. 

Põhitaseme sätte mittekohanemise kõige levinum põhjus on see, et sama sätet kasutatakse teises profiilis. Seda stsenaariumi saab konkreetse seadme puhul uurida, valides selle seadme turbe alusjoone profiili sõlmest Seadme olek. Lisateavet leiate teemast [Konfliktide lahendamine turbe alusjoonte korral.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)