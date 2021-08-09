---
title: 'AIP-skanner: installimine ja konfigureerimine'
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
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934253"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-skanner: installimine ja konfigureerimine

**AIP-skanneri installimiseks järgige soovitatud juhiseid.**

1. Kui täiendate versiooni ja ei tee puhast installi, veenduge, et olete [järginud Azure'i](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) teabekaitse skanneri ja ühtse sildistamisrakenduse versiooni täiendamise juhiseid, lugege [teemat Azure'i teabekaitse skanneri täiendamine.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Veenduge, et vastate kõigile [tulemüüride ja võrgutaristu sätete nõuetele.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Veenduge, et [poliitikad on](https://docs.microsoft.com/azure/information-protection/configure-policy) seatud automaatseks sildistuseks või et poliitikas oleks vaikesilt.
4. Veenduge, et vastav failitüüp on konfigureeritud sildi/kaitse jaoks, nagu on kirjeldatud [jaotises Azure'i teabekaitse klientrakenduse toetatud failitüübid.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Lisaks, kui soovite vaikekäitumist muuta, järgige järgmisi juhiseid. [Failide vaikekaitsetaseme muutmine.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Veenduge, et skanneriteenuse käivitamiseks konfigureeritud kasutajakontol oleks juurdepääs kõigile konfigureeritud hoidlatele.
6. Kui teil esineb endiselt probleeme, eksportige skanneri logid ja lisage need oma tugipileti.

**Azure'i teabekaitse skanneri logide eksportimine**

1. Liikuge kasutajakontekstis, kus töötab skanneriteenus, jaotisse %localappdata%\Microsoft\MSIP.
2. Zip kogu sisu alla MSIP kausta.
3. Salvestage logid oma asukohavalikusse ja manustage need oma teenusetaotlusele.
4. Samuti saate kasutada [funktsiooni Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Lisateavet leiate teemast**
- [Azure'i teabekaitse skanneri juurutamine failide automaatseks liigitamiseks ja kaitsmiseks](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Set-AIPAuthenticationi parameetri Token (Luba) määramiseks ja kasutamiseks](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Tuvastustsükli käivitamine ja skanneri aruannete kuvamine](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Azure'i teabekaitse dokumentatsiooni läbivaatamine](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure'i teabekaitse nõuded](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure'i teabekaitse kliendi allalaadimine](https://www.microsoft.com/download/details.aspx?id=53018)
