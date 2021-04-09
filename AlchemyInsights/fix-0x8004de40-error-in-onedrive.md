---
title: OneDrive 0x8004de40 i tõrke lahendamiseks
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649744"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDrive 0x8004de40 i tõrke lahendamiseks

Kui kasutate opsüsteemi Windows 7 ja teile kuvatakse see tõrketeade, värskendage [Windowsis WinHTTP-s TLS 1.1 ja TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)lubamiseks turvaliste vaikeprotokollidena.

Kui kasutate opsüsteemi Windows 10 ja teile kuvatakse OneDrive'0x8004de40 tõrketeade:

- Taaskäivitage mõjutatud arvuti, kui see on ühendatud teie Acitve'i kataloogi domeeniga.
- Kui taaskäivitamine probleemi ei lahenda, lülitage seade Azure AD-st välja ja ühinege uuesti. 

**Märkus.** Neid toiminguid tehes peaksite olema oma ettevõtte võrgus. Ärge tehke neid toiminguid, kui te pole ühendatud oma ettevõtte taristuga (nt reisil olles). 

1. Avage laiendatud käsuviip, valides **Start**, paremklõpsake käsku **Käsuviip** ja seejärel valige **Käivita administraatorina**.

1. Tippige *dsregcmd /leave ja vajutage* sisestusklahvi **(Enter).**

1. Kui see on valmis, tippige *dsregcmd /join ja* vajutage sisestusklahvi **(Enter).**

1. Kui see on valmis, sulgege käsuviip.

1. Taaskäivitage arvuti ja logige sisse OneDrive'i.