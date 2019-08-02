---
title: Rakendades meeskonnad või standalone, millel uue või olemasoleva Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054227"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Rakendades meeskonnad või standalone, millel uue või olemasoleva Office

Microsoft Teams on nüüd sisaldub toodetes ***uue installi*** Office 365 ProPlus, Office 365 Business ja Office for Mac. Lisateabe saamiseks vaadake [kui hakkab Microsoft Teams on kaasas Office selliste seadmete?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Lisaks alates versioon 1906 kuu kanalis, meeskonnad toimub ***olemasolevatele käitistele on*** Office 365 ProPlus (ja Office 365 Business) seadmeid Windows teie praegune Install versiooni uuendamisel. Lisateabe saamiseks vaadake [aga olemasolevatele käitistele on?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Kui te ei soovi oodata levikuga ajakava, saate juurutada meeskonnad standalone kasutajatele järgides [neid juhiseid](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) või lasta kasutajatel installida meeskonnad ise: [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Kui teie organisatsioon ei ole valmis kasutama meeskonnad, meil on teile tegema ***meeskonnad*** välistada [uute](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) või [olemasolevate](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) käitiste Office'i. Kui soovite installida, kuid ei taha meeskonnad pärast installimist käivitada automaatselt kasutaja, vt [Vältida Microsofti meeskonnad automaatselt pärast installi käivitumist](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)meeskonnad.

***Meeskonnad desinstallida*** seadme, kus töötab Windows, vt [Desinstallida Microsoft meeskonnad](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Cleanup Microsoft Teams mitu sihtrühma kaugmasinate või -kasutajate, vaadake [Microsofti meeskonnad juurutamine puhastada](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Kui jagate arvutit kasutades, kaugtöölaua teenuste (RDS) või Virtual Desktop infrastruktuuri (VDI), vt [jagatud arvuti ja Microsofti võistkonnad VDI keskkond](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Kasutamisel Office for Mac, vaadake [Microsofti meeskonnad seadmete Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Pärast installimist meeskonnad on [uuendatakse automaatselt](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) umbes iga kahe nädala järel, kui on uusi funktsioone ja kvaliteedi uuendused. 