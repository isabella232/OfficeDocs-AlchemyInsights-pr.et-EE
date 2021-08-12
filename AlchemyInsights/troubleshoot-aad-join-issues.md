---
title: Azure AD liitumise probleemide tõrkeotsing
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939915"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Azure AD liitumise probleemide tõrkeotsing

1. Kui häälestate seadme registreerimisi esimest korda, veenduge, et olete läbi vaadanud seadmehalduse tutvustuse [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) mis juhendab teid, kuidas azure AD-le seadmed juhtimise alla saada. 
1. Kui registreerite seadmeid otse Azure AD-sse ja registreerite need Intune'i, peate tagama, et [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) olete [Intune'i](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) konfigureerinud ja litsentsimise esmalt paika sidnud.
1. Veenduge, et teil oleks azure AD-s õigus teha toiminguid. Seadmeregistreerimiste sätteid saab hallata ainult Azure AD üldadministraator.
1. Azure AD liitumise rakendamiseks lugege teemat [Azure AD-ühenduse kavandamine.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Azure AD-ga liitumise levinumate probleemide lahendamise kohta leiate lisateavet teemast [Azure Ad Joini](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) KKK ja Windows 10 pro-seadme kohta leiate lisateavet teemast Windows 10 Pro-seadmega [Azure AD-ga liitumine –](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) vajadus üle minna – Microsofti kogukonnale
