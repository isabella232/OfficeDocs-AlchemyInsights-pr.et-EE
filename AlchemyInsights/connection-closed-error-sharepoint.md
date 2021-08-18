---
title: Aluseks olev ühendus suleti SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317692"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Tõrge "Aluseks olev ühendus suleti" SharePoint

Kui teile kuvatakse tõrketeade "Aluseks olev ühendus suleti" SharePoint võib see olla seotud TLS 1.0/1.1 deprecationiga. Lisateavet leiate nendest artiklitest.

- [TLS 1.2 ettevalmistamine Office 365 ja Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Autentimistõrked ilmnevad siis, kui kliendil pole TLS 1.2 tugit](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Värskendus TLS 1.1 ja TLS 1.2 lubamiseks winHTTP-s Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Kui kasutajad on Windows 7, veenduge, et nad märgivad [TLS-i šifri komplektid Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)