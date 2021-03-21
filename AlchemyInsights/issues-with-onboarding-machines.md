---
title: Probleemid arvutite ühendamisel Microsoft Defender for Endpointsiga
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901563"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Probleemid arvutite ühendamisel Microsoft Defender for Endpointsiga

Võib-olla on teil probleeme arvutite ühendamisega MDE teenusega. Kui pääsete juurde lõppkasutaja arvutile, tehke järgmist:

1. Laadige alla [MDE kliendianalüsaatori](https://aka.ms/betamdeanalyzer) diagnostika tööriista uusim eelvaate versioon.
2. Paremklõpsake failil **MDEClientAnalyzer.cmd** ja valige käsk "Käivita administraatorina".
3. Järgige juhiseid, mida on soovitatud **MDEClientAnalyzer.htm**.
4. Paljusõnaliste logide vaatamiseks vaadake loodud alamkausta nimega **MDEClientAnalyzerResult**.
5. Kui on vaja täiendavaid juhiseid, pöörduge [Microsoft Defender for Endpoint kasutajatoe](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) poole ja esitage analüüsiks fail MDEClientAnalyzerResult.zip.
