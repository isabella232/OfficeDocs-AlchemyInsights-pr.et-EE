---
title: Office ' i rakenduste värskendamise kanalite muutmine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439018"
---
# <a name="change-update-channels-for-office-apps"></a>Office ' i rakenduste värskendamise kanalite muutmine

Uute Office ' i installide korral kasutage soovitud värskendamise kanali valimiseks Office ' i tarkvara allalaadimise sätteid ja seejärel installige (või installige uuesti) Office ' i rakendused. Lisateavet leiate teemast [tarkvara allalaadimise sätete haldamine rakenduses Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Märkus** Office ' i tarkvara allalaadimise sätete abil valitud kanali Update kehtib kõigi kasutajate jaoks, kes kasutavad O365 portaali kaudu uusi installe. Lisateavet leiate teemast [Microsoft 365 või Office 2019 allalaadimine ja installimine või uuesti installimine PC-või Mac-arvutisse](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Olemasolevate Office ' i installide jaoks kasutage Office ' i juurutamise tööriista (ODT) mõne muu värskendamise kanali aktiveerimiseks.  

1. Laadige [Microsofti allalaadimiskeskusest](https://go.microsoft.com/fwlink/p/?LinkID=626065)alla Office ' i juurutamise tööriista (setup.exe) uusim versioon.
2. Määrake kanali nimi, mille soovite aktiveerida. Lisateavet leiate teemast [Office ' i juurutamise tööriista konfiguratsiooni suvandid](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Saate luua konfiguratsiooni XML-faili, mis määrab vastava kanali nime (nt update.xml).  
    loomine. <Configuration>  
    b. <uuendused **Channel = "kuu"** />  
    c. </Configuration>
4. Liikuge tõstetud käsuviiba kaudu kausta asukohta, kus setup.exe asub, ja käivitage järgmine käsk.  
    loomine. setup.exe/Configure update.xml
5. Käivitage Office ' i rakendus (nt Excel) ja valige **siis käsk "**  >  **konto**". **Valige jaotises tootekirjeldus nupp Värskenda**  >  **kohe**.

Lisateavet leiate teemast [olemasolevate Office ' i rakenduste värskendamise kanalite vahetamine](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Valitud kasutajate rühma värskenduste vahetamiseks või Configuration Manageri (SCCM) häälestamiseks Konfigureerige rühma "GPO" abil säte Värskenda kanal. Lisateavet leiate teemast [Microsoft 365 rakenduste värskendamise kanalite ülevaade](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Lisateavet leiate teemast [Office 365 ProPlus kanalite haldamine IT-spetsialistidele](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) ja [Microsoft 365 rakenduste värskenduste haldamine Microsoft Endpoint Configuration Manageri abil](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).