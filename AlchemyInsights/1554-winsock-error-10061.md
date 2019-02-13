---
title: 1554 Winsock-tõrge 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903092"
---
# <a name="winsock-error-10061"></a>Winsocki tõrge 10061

See tähendab, et Office 365 ei saanud luua TCP pesa (ühendus) Sihthosti. Selle tõrke põhjuseks enamasti oma tulemüüri konfiguratsiooni osas probleemi. Probleemi lahendamiseks kontrollige neid sätteid:
  
- Kontrollige oma tulemüüri konfiguratsiooni teabe [Office 365 URL-id](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) ja IP-aadressid
    
- Kui viga ilmneb et Exchange Online kaitse (EOP), sa peaks on varem teatatud muudatusi [Exchange Online kaitse IP-aadressid](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Veenduge, et teie Interneti-teenuse pakkuja (ISP) ei blokeeri sadama.
    
- Nutika hosti ja sihtarvutite serveri sätteid oma pistikud kontrollida.
    
Pange tähele, et Office 365 ei blokeerida *sissetulevad* ühendused sel viisil. 
  

