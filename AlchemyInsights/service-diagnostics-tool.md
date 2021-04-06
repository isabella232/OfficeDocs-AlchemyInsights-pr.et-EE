---
title: Windows Virtual Desktopi teenusediagnostika tööriist
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595632"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windows Virtual Desktopi teenusediagnostika tööriist

Windows Virtual Desktop (WVD) pakub diagnostikatööriista, mis võimaldab administraatoritel tuvastada tõrkeid ühe liidese kaudu. See tööriist logib diagnostikaga seotud teavet iga kord, kui WVD-d kasutab keegi, kellele on määratud WVD roll. Iga logi sisaldab teavet tegevusega seotud WVD rolli, seansi ajal kuvatavate tõrketeadete ning rentniku ja kasutaja kohta. Azure'i logianalüüsi saab konfigureerida jäädvustama diagnostikatööriista loodud tegevuste logi, järgides järgmisi juhiseid.

1. Logianalüüsi tööruumi loomine [Azure'i portaali või](https://go.microsoft.com/fwlink/?linkid=2129500) [Azure PowerShelli abil.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Ühendage Windowsi arvutid Azure'i kuvariga.](https://go.microsoft.com/fwlink/?linkid=2129913) Hankige tööruumi ID ja tööruumi primaarvõti. Häälestusviisard vajab seda teavet agendi õigeks konfigureerimiseks ja Azure Monitoriga suhtlemiseks.

1. [Lükake diagnostikaandmed oma tööruumi.](https://go.microsoft.com/fwlink/?linkid=2128284) Saate oma WVD rentniku diagnostikaandmed oma tööruumi logianalüüsisse lükata.

1. [Tuvastage ja diagnoosige probleeme,](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) mis on WVD-ga seoses sisemised või välisprobleemid.

Lisateavet WVD teenusediagnostikatööriista konfigureerimise kohta leiate teemast Logianalüüsi kasutamine diagnostikafunktsiooni jaoks.