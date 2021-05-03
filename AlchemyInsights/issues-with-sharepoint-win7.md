---
title: Probleemid SharePoint 7 Windows seadmetega
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
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125119"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Probleemid SharePoint 7 Windows seadmetega

Kui teile kuvatakse tõrkeid Windows 7-s SharePoint või OneDrive, võivad need olla seotud TLS 1.0/1.1 deprecationiga. Lisateavet leiate järgmistest teemadest.

- [TLS 1.2 ettevalmistamine Office 365 ja Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 peab TLS1.2 olema lubatud. Lisateavet leiate teemast [Autentimistõrked, kui klientrakendusel pole TLS 1.2 tugit](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Installige KB3140245 ja looge registriväärtus. Lisateavet leiate teemast [Värskendus TLS 1.1 ja TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) lubamiseks winHTTP-s Windows

- Windows 7 SP1/Windows 8 klient peab tagama uusimate TLS-i šifri komplektide installimise. Lisateavet leiate teemast [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


