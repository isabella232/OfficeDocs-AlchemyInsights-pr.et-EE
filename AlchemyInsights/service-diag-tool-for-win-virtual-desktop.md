---
title: Teenuse diagnostika tööriist Windows Virtual Desktopi jaoks
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677651"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Teenuse diagnostika tööriist Windows Virtual Desktopi jaoks

Windowsi Virtual Desktop (WVD) pakub diagnostilist tööriista, mis võimaldab administraatoritel tuvastada tõrkeid ühe liidese kaudu. See tööriist logib diagnostikaga seotud teavet alati, kui WVD kasutab keegi, kellele on määratud WVD roll. Iga logi sisaldab teavet tegevusega seotud WVD rolli, seansi ajal kuvatavate tõrketeadete ning rentniku ja kasutaja kohta käiva teabe kohta. Azure ' i Logi analüüsi saab konfigureerida, et jäädvustada diagnostiline tööriist loodud tegevuste Logi. Tehke järgmist.

1. Azure ' i [portaali](https://go.microsoft.com/fwlink/?linkid=2129500) või [Azure PowerShelli](https://go.microsoft.com/fwlink/?linkid=2129501)abil saate luua Logi Analyticsi tööruumi.
1. [Ühendage Windowsi arvutid Azure ' i kuvariga](https://go.microsoft.com/fwlink/?linkid=2129913). Hankige tööruumi ID ja oma tööruumi primaarvõti. Installiviisard vajab seda teavet agendi õigeks konfigureerimiseks ning selle tagamiseks, et see saaks suhelda Azure ' i kuvariga.
1. [Push diagnostika andmed oma tööruumi](https://go.microsoft.com/fwlink/?linkid=2128284). Saate WVD rentniku andmeid oma tööruumi Logi analüüsile üle anda.
1. WVD seotud sisemiste või väliste [probleemide tuvastamine ja diagnoosimine](https://go.microsoft.com/fwlink/?linkid=2128338) .

Lisateavet WVD teenuse diagnostika tööriista konfigureerimise kohta leiate teemast [diagnostika funktsiooni jaoks Logi analüüsi kasutamine](https://go.microsoft.com/fwlink/?linkid=2128084).
