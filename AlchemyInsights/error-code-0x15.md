---
title: Tõrkekood 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Kui Office 2013 aktiveerimisel kaugtöölaua teenuste (RDS) juurutustes kuvatakse tõrketeade, kaaluge ADAL lubamist registri redigeerimise teel.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709183"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Office 2013 aktiveerimisel Remote Desktop Services tõrge

Kui Office 2013 aktiveerimisel kaugtöölaua teenuste (RDS) juurutustes kuvatakse tõrketeade, kaaluge ADAL lubamist registri redigeerimise teel.
  
|**Registrivõti**|**Tüüp**|**Väärtus**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Lisateavet leiate teemast [Office 2013 modernse autentimise lubamine Windowsi seadmetes](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Microsoft 365 rakendustes Enterprise and Office 2016 on ADAL vaikimisi lubatud. Kaugtöölaua teenused (RDS) kasutasid varem terminaliteenuste nime.
  