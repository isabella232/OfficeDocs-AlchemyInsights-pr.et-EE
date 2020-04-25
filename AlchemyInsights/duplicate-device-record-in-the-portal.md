---
title: Portaalis seadme kirje dubleerimine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789685"
---
# <a name="duplicate-device-record-in-the-portal"></a>Portaalis seadme kirje dubleerimine

Kui seade ei raporteeri Configuration Manageri saidile kaashalduse olekut õigesti, võite näha portaalis seadme jaoks kahte kirjet. Seadme kaashalduse oleku kontrollimiseks vaadake Configuration Manageri konsoolis seadme veergu **Kaashallatud**. Kui veerg pole nähtav, võite selle lisada, paremklõpsates mõnda veerupäist ja valides selle loendist.

Suvandi Kaashallatav väärtus peab olema **Jah**. Kui väärtus on **Ei**, avage klientrakenduses Configuration Manageri kliendi aplett ja kontrollige vahekaardil Üldine atribuuti **Kaashaldus**.

- Kui väärtus on **Lubatud**, näitab see halduspunkti kliendisuhtuse probleeme. Vaadake seadmes logi **CcmMessaging.log**, et uurida võimalikke ühenduvuse probleeme.

- Kui väärtus on **Keelatud** ja seade on registreeritud Intune’is, veenduge, et seade oleks saanud kaashalduse poliitika, vaadates seadmes läbi logi **CoManagementHandler.log**.
