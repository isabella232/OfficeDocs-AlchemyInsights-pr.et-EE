---
title: Probleemid sisselogimisel Microsoft 365 rakendustesse
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744632"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Sisselogimisega seotud Microsoft 365 rakendused

Märkus. Kui kasutate versiooni Windows (nt Windows 7 SP1, Windows Server 2008 R2) vanemat versiooni, [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) kasutage funktsiooni TLS 1.2 vaikimisi lubamiseks parandust. Lisateavet leiate teemast [Värskendus TLS 1.1 ja TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)lubamiseks WinHTTP-s Windows.

Microsoft 365 rakendustesse sisselogimisega seotud probleemide lahendamiseks proovige probleemses arvutis järgmisi toiminguid:  

- Lisateavet Windows teemast [Soovitused levinud sisselogimisprobleemide](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) lahendamise kohta.
- Mac-arvutis leiate lisateavet teemast Ei saa Office [2016 for Maci rakendusse sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Näpunäide** Windowsi seadmetes saame diagnoosida ja automaatselt lahendada mitmed levinud Office'i sisselogimisprobleeme. Meie automatiseeritud tööriista kasutamiseks laadige alla ja käivitage **[Microsofti tugi- ja taasteteenuste abiline](https://aka.ms/SaRA-OfficeSignInScenario)**.

**Märkus.** Modernautentimise (ADAL) või veebikonto halduse (WAM) keelamine sisselogimise või aktiveerimisega seotud probleemide **lahendamiseks pole soovitatav.** Kui tõrked ilmnevad ühenduse loomisel Microsoft 365 2013 Office, veenduge, [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) et lubate Office autentimise.

Konkreetsete tõrkeotsingutoimingute kohta leiate lisateavet teemast

[Pärast 2016. aasta Office järgus 16.0.7967 sisselogimisprobleeme Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Te ei saa oma organisatsioonikontosse (nt Office 365, Azure'i ega Intune'i) sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Mittebrauserirakenduste tõrkeotsing, mis ei saa Office 365, Azure'i või Intune'i](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Korduvalt küsitakse identimisteavet Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)