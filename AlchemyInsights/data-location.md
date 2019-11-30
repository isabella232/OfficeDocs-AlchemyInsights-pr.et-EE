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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627842"
---
# <a name="data-location"></a>Andmete asukoht

Saate vaadata oma Office 365 rentniku asukoht administreerimiskeskuses või ühendust Exchange Online PowerShelli kaudu.


**Halduskeskus:**
1. Logige sisse [administreerimiskeskusesse](https://admin.microsoft.com/Adminportal/Home).
2. Valige **sätted** > **organisatsiooni profiil**.
3. Valige jaotises **andmete asukoht** **Kuva üksikasjad**.


**Powershelli:**
1. Windows PowerShelli abil ühendust Exchange Online ' i.
2. Käivitage cmdlet [-käsu Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) , et kuvada teie rentniku atribuutide loend. 
3. Vaadake atribuuti OrganizationId.

Kui teil on EXO ja SPO andmete asukoht, saate määrata andmete asukoha muude teenuste kohta, mida te [oma andmete](https://products.office.com/where-is-your-data-located)asukoha puhul kasutada võite.