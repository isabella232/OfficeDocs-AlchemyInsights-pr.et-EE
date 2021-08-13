---
title: Azure AD hübriidjuurutusega liitumise tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939267"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Azure AD hübriidjuurutusega liitumise tõrkeotsing

Tungivalt soovitatav: veenduge, et seade pääseks juurde süsteemikontol määratud seadmete registreerimise lõpp-punktidele. Selleks kasutage [seadme registreerimise ühenduvuse testimise skripti](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Kui häälestate seadmeregistreerimisi esmakordselt, vaadake kindlasti läbi ka [Azure Active Directory seadmehaldus tutvustus](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), kust leiate lisateavet selle kohta, kuidas tuua seadmed Azure AD kontrolli alla.
1. Kui registreerite seadmeid Azure AD-sse otse ning lisaks registreerite need ka Intune‘is, veenduge esmalt, et [Intune oleks konfigureeritud](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ja teil oleks olemas õiged [litsentsid](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Veenduge, et teil oleks õigus teha toiminguid nii Azure AD-s kui ka kohapealses AD-s. Seadmeregistreerimiste sätteid saab hallata ainult Azure AD üldadministraator. Kui häälestate automaatseid registreerimisi oma kohapealses Active Directorys, peate lisaks olema ka Active Directory ja AD FS-i (kui see on asjakohane) administraator.

Lisateavet hübriidjuurutusega liitumise potentsiaalsete probleemide lahendamise kohta leiate siit: [Hübriidjuurutusega liitumise tõrkeotsing](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Kui soovite häälestada Azure AD hübriidjuurutusega liitumise ning hallata seadmeid Azure AD portaali kaudu, lugege artikleid [Seadmete Azure AD hübriidjuurutuses (kohapealses domeenis) kasutuselevõtu liitumise häälestamine](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) ja [Seadmete haldamine Azure‘i portaali kaudu](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Azure Active Directory (AD) hübriidjuurutusega liitumise levinud probleemide tõrkeotsingu tegemiseks lugege artiklit [Azure AD hübriidjuurutusega liitumise KKK](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
