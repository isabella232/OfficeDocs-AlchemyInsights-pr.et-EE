---
title: Teenuse diagnostikatööriist virtuaalse Windows jaoks
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052382"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Teenuse diagnostikatööriist virtuaalse Windows jaoks

Windows Virtuaaltöölaud (WVD) pakub diagnostikatööriista, mis võimaldab administraatoritel tuvastada tõrkeid ühe liidese kaudu. See tööriist logib diagnostikaga seotud teavet iga kord, kui WVD-d kasutab keegi, kellele on määratud WVD roll. Iga logi sisaldab teavet tegevusega seotud WVD rolli, seansi ajal kuvatavate tõrketeadete ning rentniku ja kasutaja kohta. Azure'i logianalüüsi saab konfigureerida jäädvustama diagnostikatööriista loodud tegevuste logi. Tehke järgmist.

1. Logianalüüsi tööruumi loomine [Azure'i portaali või](https://go.microsoft.com/fwlink/?linkid=2129500) [Azure PowerShelli abil.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Ühendus Windows azure'i kuvarisse.](https://go.microsoft.com/fwlink/?linkid=2129913) Hankige tööruumi ID ja tööruumi primaarvõti. Häälestusviisard vajab seda teavet agendi õigeks konfigureerimiseks ja Azure Monitoriga suhtlemiseks.
1. [Lükake diagnostikaandmed oma tööruumi.](https://go.microsoft.com/fwlink/?linkid=2128284) Saate oma WVD rentniku diagnostikaandmed oma tööruumi logianalüüsisse lükata.
1. [Tuvastage ja diagnoosige probleeme, mis](https://go.microsoft.com/fwlink/?linkid=2128338) on WVD-ga seoses sisemised või välisprobleemid.

Lisateavet WVD teenusediagnostikatööriista konfigureerimise kohta leiate teemast [Logianalüüsi kasutamine diagnostikafunktsiooni jaoks.](https://go.microsoft.com/fwlink/?linkid=2128084)
