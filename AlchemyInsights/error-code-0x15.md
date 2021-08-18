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
description: Kui teenuse Remote Desktop Services (RDS) Office 2013 aktiveerimisel ilmneb tõrge, kaaluge registri redigeerimise abil ADAL-i lubamist.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316682"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Tõrge kaugtöölaua teenustes Office 2013 aktiveerimisel

Kui teenuse Remote Desktop Services (RDS) Office 2013 aktiveerimisel ilmneb tõrge, kaaluge registri redigeerimise abil ADAL-i lubamist.
  
|**Registrivõti**|**Tüüp**|**Väärtus**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Lisateavet leiate teemast [Modernautentimise lubamine Office 2013 Windows seadmetes.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Märkus.** ADAL on vaikimisi lubatud Microsoft 365 suurettevõtterakendused ja Office 2016. Kaugtöölaua teenuste (RDS) nimi oli varem terminaliteenused.
  