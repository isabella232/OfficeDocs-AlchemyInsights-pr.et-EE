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
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814512"
---
# <a name="duplicate-device-record-in-the-portal"></a>Portaalis seadme kirje dubleerimine

Kui seade ei raporteeri Configuration Manageri saidile kaashalduse olekut õigesti, võite näha portaalis seadme jaoks kahte kirjet. Seadme kaashalduse oleku kontrollimiseks vaadake Configuration Manageri konsoolis seadme veergu **Kaashallatud**. Kui veerg pole nähtav, võite selle lisada, paremklõpsates mõnda veerupäist ja valides selle loendist.

Suvandi Kaashallatav väärtus peab olema **Jah**. Kui väärtus on **Ei**, avage klientrakenduses Configuration Manageri kliendi aplett ja kontrollige vahekaardil Üldine atribuuti **Kaashaldus**.

- Kui väärtus on **Lubatud**, näitab see halduspunkti kliendisuhtuse probleeme. Vaadake seadmes logi **CcmMessaging.log**, et uurida võimalikke ühenduvuse probleeme.

- Kui väärtus on **Keelatud** ja seade on registreeritud Intune’is, veenduge, et seade oleks saanud kaashalduse poliitika, vaadates seadmes läbi logi **CoManagementHandler.log**.
