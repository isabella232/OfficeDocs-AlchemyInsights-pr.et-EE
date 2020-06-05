---
title: Probleemid sisselogimisel Microsoft 365 rakendused
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579897"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tühi sisselogimiskuva rakenduses Microsoft 365 rakendused

Selle probleemi lahendamiseks proovige järgmist.
- Installige uusimad värskendused [Windowsi](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office ' i](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)jaoks.
- Lähtesta Internet Exploreri suvandid: **tööriistadele**  >  **Interneti-suvandid**  >  **Täpsemad**  >  **Lähtesta Internet Exploreri sätted** (Pange tähele, et kaotate kohandatud sätted) ja seejärel proovige uuesti Office ' i sisse logida.
- Keelake Windows Defenderi Rakendusevalvur (WDAG) või muu sarnane tulemüür või viirusetõrje programm:
    1. Juhtpaneel, avage **programmid**ja seejärel valige **Lülita Windowsi funktsioonid sisse või välja**.
    2. Kui Windows Defenderi Rakendusevalvur on lubatud, proovige seda keelata.<br/>
    **Märkus:** Võimalik, et peate arvuti taaskäivitama.
- Veenduge, et Microsoft. AAD. vahendajate plugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ei ole blokeeritud ühtegi rakendust või tulemüüri/viirusetõrje programm.
- [Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , kasutades Windowsi mandaat Manager.<br/>
    **Märkus:** Office 2016 registri teed on muutunud 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Lisateabe saamiseks vaadake [ühenduse probleemid sisse logida pärast värskenduse Office 2016 ehitada 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).