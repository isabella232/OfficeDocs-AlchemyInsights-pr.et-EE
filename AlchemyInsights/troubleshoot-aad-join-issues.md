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
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404631"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Azure AD liitumise probleemide tõrkeotsing

1. Kui häälestate seadme registreerimisi esimest korda, veenduge, et olete läbi vaadanud [Azure Active Directorys](https://docs.microsoft.com/azure/active-directory/devices/overview) seadmehalduse tutvustuse, mis juhendab teid, kuidas azure AD-le seadmed kontrolli alla saada. 
1. Kui registreerite seadmeid otse Azure AD-sse ja registreerite need Intune'i, peate tagama, et [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) olete [Intune'i](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) konfigureerinud ja litsentsimise esmalt paika sidnud.
1. Veenduge, et teil oleks azure AD-s õigus teha toiminguid. Ainult Azure AD üldadministraator saab hallata seadme registreerimise sätteid.
1. Azure AD liitumise rakendamiseks lugege teemat [Azure AD-ühenduse kavandamine.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Azure AD-ga liitumise levinumate probleemide lahendamise kohta leiate lisateavet teemast [Azure Ad Joini](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) KKK ja Windows 10 pro seadme kohta leiate lisateavet teemast Windows 10 Pro seadmega [Azure AD-ga](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) liitumine – üleminek Microsofti kogukonnale
