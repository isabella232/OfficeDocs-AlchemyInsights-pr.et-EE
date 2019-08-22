---
title: Tõrkekood 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Kui teile kuvatakse tõrge aktiveerides Office 2013 kaugtöölaua teenuste (RDS) kasutuselevõttu, kaaluma skeeme ADAL registri.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526983"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Kaugtöölaua teenuste aktiveerimise Office 2013 ilmnes tõrge

Kui teile kuvatakse tõrge aktiveerides Office 2013 kaugtöölaua teenuste (RDS) kasutuselevõttu, kaaluma skeeme ADAL registri.
  
|**Registrivõtme**|**Tüüp**|**Väärtus**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Lisateabe saamiseks vt [Office 2013 Windowsi seadmete lubade kasutada programmi kaasaegne autentimine](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Office 365 ProPlus ja Office 2016 on lubatud ADAL. Kaugtöölaua teenused (RDS) nimetati varem Terminal Services.
  