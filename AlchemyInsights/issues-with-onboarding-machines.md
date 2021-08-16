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
ms.openlocfilehash: 5f2ed08e32694a6d7293abbabb1eddd3d251ceddbd9debf6ec3143bb4fed86db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054686"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Probleemid arvutite ühendamisel Microsoft Defender for Endpointsiga

Võib-olla on teil probleeme arvutite ühendamisega MDE teenusega. Kui pääsete juurde lõppkasutaja arvutile, tehke järgmist:

1. Laadige alla [MDE kliendianalüsaatori](https://aka.ms/betamdeanalyzer) diagnostika tööriista uusim eelvaate versioon.
2. Paremklõpsake failil **MDEClientAnalyzer.cmd** ja valige käsk "Käivita administraatorina".
3. Järgige juhiseid, mida on soovitatud **MDEClientAnalyzer.htm**.
4. Paljusõnaliste logide vaatamiseks vaadake loodud alamkausta nimega **MDEClientAnalyzerResult**.
5. Kui on vaja täiendavaid juhiseid, pöörduge [Microsoft Defender for Endpoint kasutajatoe](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) poole ja esitage analüüsiks fail MDEClientAnalyzerResult.zip.
