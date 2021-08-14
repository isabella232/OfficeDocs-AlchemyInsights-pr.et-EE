---
title: Portaalis seadme kirje dubleerimine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004150"
---
# <a name="duplicate-device-record-in-the-portal"></a>Portaalis seadme kirje dubleerimine

Kui seade ei raporteeri Configuration Manageri saidile kaashalduse olekut õigesti, võite näha portaalis seadme jaoks kahte kirjet. Seadme kaashalduse oleku kontrollimiseks vaadake Configuration Manageri konsoolis seadme veergu **Kaashallatud**. Kui veerg pole nähtav, võite selle lisada, paremklõpsates mõnda veerupäist ja valides selle loendist.

Suvandi Kaashallatav väärtus peab olema **Jah**. Kui väärtus on **Ei**, avage klientrakenduses Configuration Manageri kliendi aplett ja kontrollige vahekaardil Üldine atribuuti **Kaashaldus**.

- Kui väärtus on **Lubatud**, näitab see halduspunkti kliendisuhtuse probleeme. Vaadake seadmes logi **CcmMessaging.log**, et uurida võimalikke ühenduvuse probleeme.

- Kui väärtus on **Keelatud** ja seade on registreeritud Intune’is, veenduge, et seade oleks saanud kaashalduse poliitika, vaadates seadmes läbi logi **CoManagementHandler.log**.
