---
title: Meeskondade juurutamine autonoomseks või uute või olemasolevate Office ' i installide puhul
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: ffa91eaf333792af149feda25f9a377ed591b597
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010214"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Meeskondade juurutamine autonoomseks või uute või olemasolevate Office ' i installide puhul

Microsoft Teams on nüüd kaasatud ***uue installi*** Microsoft 365 apps Enterprise, Microsoft 365 rakendused äri ja Office for Mac. Lisateabe saamiseks vaadake, [Millal Microsoft Teams hakkavad sisalduma Office ' i uute installide puhul?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Lisaks alates versioon 1906 igakuine kanal, meeskonnad ***lisatakse olemasolevatele installid*** Microsoft 365 apps Enterprise (ja Microsoft 365 apps ettevõtetele) seadmetes, kus töötab Windows, kui värskendate olemasoleva installi uusim versioon. Lisateabe saamiseks vaadake, [mis on Office ' i olemasolevate installide kohta?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Kui te ei soovi selle rollout ajakava oodata, saate juurutada meeskonnad autonoomseks oma kasutajatele, [järgides neid juhiseid](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) või saate lasta oma kasutajatel installida meeskonnad ise [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Kui teie organisatsioon pole meeskondi juurutamiseks valmis, on meil sammud, mida saate võtta, et ***välistada meeskonnad*** [uutest](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) või [olemasolevatest](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installid. Kui soovite meeskondi installida, kuid ei soovi, et meeskonnad käivituma kasutaja jaoks automaatselt pärast selle installimist, vaadake teemat [Microsofti meeskondade automaatse installimise vältimine](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***Meeskondade desinstallimiseks*** seadmest, milles töötab Windows, vaadake teemat [Microsoft teamsi desinstallimine](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Microsoft Teamsi puhastamiseks mitmest sihtmasinast või kasutajalt vaadake teemat [Microsoft teamsi juurutamine puhastada](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Kui kasutate ühiskasutatavat arvutit, kaugtöölaua teenuseid (RDS) või virtuaalse töölaua taristut (VDI), vaadake [Microsoft Teamsi ühiskasutatavat arvutit ja VDI keskkonda](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Kui kasutate Office for Mac, vaadake [Microsoft teamsi installi Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Kui meeskonnad on installitud, värskendatakse see [automaatselt](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) umbes iga kahe nädala järel uute funktsioonide ja kvaliteedivärskendustega. 