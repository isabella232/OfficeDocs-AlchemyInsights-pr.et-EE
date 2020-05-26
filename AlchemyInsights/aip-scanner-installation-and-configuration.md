---
title: 'AIP-skanner: paigaldamine ja konfigureerimine'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357661"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-skanner: paigaldamine ja konfigureerimine

**AIP skanneri installimiseks järgige soovitatud juhiseid**.

1. Kui täiendate ja ei tee puhast installi, veenduge, et olete järginud juhiseid [Azure ' i teabe kaitse skanneri](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ja ühendatud märgistamise kliendi täiendamine, vaadake [Azure ' i teabe kaitse skanneri täiendamine](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Veenduge, et te järgite kõiki [tulemüüride ja võrgu infrastruktuuri seadete nõudeid](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Veenduge, et teie [poliitikad on seatud](https://docs.microsoft.com/azure/information-protection/configure-policy) automaatne märgistamine või on vaikimisi silt poliitika.
4. Veenduge, et vastav failitüüp on konfigureeritud sildi/kaitse puhul, nagu on kirjeldatud [Azure ' i teabekaitse kliendi toetatud failitüüpide](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)puhul. Lisaks, kui soovite muuta vaikekäitumist, järgige neid juhiseid: [muuta failide vaikimisi kaitse tase](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Veenduge, et skanneri teenuse käivitamiseks konfigureeritud kasutajakontole on juurdepääsuõigused kõigile konfigureeritud hoidlates.
6. Kui teil esineb endiselt probleeme, siis eksportike skanneri logid ja lisage need oma toe pilet.

**Ekspordi Azure ' i teabe kaitse skanner logid**

1. Liikuge%localappdata%\Microsoft\MSIP skanneri teenust käitavas kasutajakonteksti all.
2. ZIP kogu sisu MSIP kausta.
3. Salvestage logid oma asukoha valikule ja kinnitage need oma teenustaotlusele.
4. Võite kasutada ka [ekspordi-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Lisateabe saamiseks vt**:
- [Azure ' i teabekaitse skanneri juurutamine failide automaatseks klassifitseerimiseks ja kaitsmiseks](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Määrake ja kasutage Set-AIPAuthentication loa parameeter](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Tuvastustsükli käivitamine ja skanneri aruannete vaatamine](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Azure ' i teabekaitse dokumentatsiooni läbivaatamine](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure ' i teabekaitse nõuded](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Laadige alla Azure ' i teabekaitse klient](https://www.microsoft.com/download/details.aspx?id=53018)
