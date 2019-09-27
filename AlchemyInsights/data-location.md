---
title: Andmete asukoht
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207257"
---
# <a name="data-location"></a>Andmete asukoht

Saate vaadata oma Office 365 rentniku asukoht administreerimiskeskuses või ühendust Exchange Online PowerShelli kaudu.


**Halduskeskus:**
1. Logige sisse [administreerimiskeskusesse](https://admin.microsoft.com/Adminportal/Home).
2. Valige **sätted** > **organisatsiooni profiil**.
3. Valige jaotises **andmete asukoht** **Kuva üksikasjad**.


**Powershelli:**
1. Windows PowerShelli abil ühendust Exchange Online ' i.
2. Käivitage cmdlet [-käsu Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) , et kuvada teie rentniku atribuutide loend. 
3. Vaadake atribuuti OrganizationId.

Kui teil on EXO ja SPO andmete asukoht, saate määrata andmete asukoha muude teenuste kohta, mida te [oma andmete](https://products.office.com/where-is-your-data-located)asukoha puhul kasutada võite.