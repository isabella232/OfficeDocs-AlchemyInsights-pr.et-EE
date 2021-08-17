---
title: 401 Volitamata tõrge SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890262"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Volitamata tõrge SharePoint

Kui kuvatakse tõrketeade "(401) Volitamata" SharePoint see võib olla seotud TLS 1.0/1.1 deprecationiga. Lisateavet leiate järgmistest artiklitest:

- [TLS 1.2 ettevalmistamine Office 365 ja Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Autentimistõrked ilmnevad siis, kui kliendil pole TLS 1.2 tugit](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Värskendus TLS 1.1 ja TLS 1.2 lubamiseks winHTTP-s Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Kui kasutajal on Windows 7, kontrollige, kas nad märgivad [TLS-i šifri komplektid Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)