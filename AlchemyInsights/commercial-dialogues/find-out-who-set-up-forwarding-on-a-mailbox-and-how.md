---
title: Uurige, kes on postkastis edasisaatmise häälestanud ja kuidas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988176"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Uurige, kes on postkastis edasisaatmise häälestanud ja kuidas

Kui väline edasisuunamine oli postkastis määratud, auditeeritakse tegevust cmdlet-käsu Set-Mailbox osana. Tegevuste leidmiseks auditilogist saate teha nii:

1. Avage Office 365 [& vastavuskeskus.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Valige **Otsi** >  **auditilogi otsingut**.
    > [!NOTE]
    > Kui näete teadet, et peate auditeerimise sisse lülitama, lülitage see kohe sisse. Kui see funktsioon pole sisse lülitatud, ei saa otsingutulemid eelmistest kuupäevadest andmeid tõmmata.
1. Veenduge, et **välja Tegevused** väärtuseks oleks määratud Kuva kõigi **tegevuste tulemid** (vaikesäte). Määrake kuupäevavahemik. Kasutajanime pole vaja määrata.
1. Valige **Otsi**. Tegevused kuvatakse jaotises **Tulemid.**
1. Valige **Filtreeri tulemid** ja seejärel **sisestage väljale** Tegevuse filter väärtus **Sea** postkast. See tagastab kõik **Set-Mailboxi tegevused.**
1. Üksikasjade kuvamiseks valige soovitud tegevus ja seejärel valige **Lisateave**. Jaotises **Parameetrid** näete postkastis määratud edasisaatmismeiliaadressi. **UserID** tähistab kasutajat, kes häälestas postkastis välise edasisaatmise.
Lisateavet leiate teemast Office 365 [auditilogist levinumate stsenaariumide tõrkeotsinguks.](https://go.microsoft.com/fwlink/?linkid=2103944)