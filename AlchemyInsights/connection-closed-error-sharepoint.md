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
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044408"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Tõrge "The underlying connection was closed" ("Aluseks olev ühendus suleti" SharePoint

Kui teile kuvatakse tõrketeade "Aluseks olev ühendus suleti" SharePoint võib see olla seotud TLS 1.0/1.1 deprecationiga. Lisateavet leiate nendest artiklitest.

- [TLS 1.2 ettevalmistamine Office 365 ja Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Autentimistõrked ilmnevad siis, kui kliendil pole TLS 1.2 tugit](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Värskendus TLS 1.1 ja TLS 1.2 lubamiseks winHTTP-s Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Kui kasutajal on Windows 7, kontrollige, kas nad märgivad [TLS-i šifri komplektid Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)