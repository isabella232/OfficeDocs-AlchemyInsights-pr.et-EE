---
title: Tõrkekood 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Kui te saate viga aktiveerides Office 2013 kaugtöölaua teenuste (RDS) kasutuselevõttu, kaaluge ADAL lubamine registri redigeerimisel.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703134"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Tõrge Office 2013 aktiveerimine kaugtöölaua teenuste

Kui te saate viga aktiveerides Office 2013 kaugtöölaua teenuste (RDS) kasutuselevõttu, kaaluge ADAL lubamine registri redigeerimisel.
  
|**Registri võti**|**Tüüp**|**Väärtus**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Lisateabe saamiseks vaadake [lubamine kaasaegne autentimine Office 2013 Windowsi seadmetes](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL on vaikimisi lubatud Microsoft 365 apps Enterprise ja Office 2016. Kaugtöölaua teenuste (RDS) oli varem nimega Terminal Services.
  