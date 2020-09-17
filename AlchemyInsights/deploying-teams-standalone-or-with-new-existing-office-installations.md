---
title: Töörühmade juurutamine eraldiseisvana või uute või olemasolevate Office ' i installide abil
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806755"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Töörühmade juurutamine eraldiseisvana või uute või olemasolevate Office ' i installide abil

Microsoft Teams on nüüd kaasatud Microsoft 365 rakenduste ***uute käitiste*** osana Enterprise ' i, Microsoft 365 rakenduste jaoks ja Office for Macile. Lisateavet leiate teemast [Millal Microsoft teamsi kaasatakse uutesse Office ' i seadmetesse?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Lisaks praeguse kanali versioonist 1906, lisatakse meeskonnad olemasolevatele seadmetele Microsoft 365 rakenduste Enterprise ' i (ja Microsoft 365 rakenduste jaoks) ***olemasolevatesse*** seadmetesse, kui värskendate olemasolevat installi uusimale versioonile. Lisateavet leiate teemast [mis saab Office ' i olemasolevatest seadmetest?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Kui te ei soovi seda levikuga seotud ajakava oodata, saate töörühmad oma kasutajate jaoks iseseisvalt juurutada, järgides [neid juhiseid](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   või saate lasta kasutajatel meeskonda ise installida  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Kui teie asutuses pole töörühma juurutamiseks valmis, on meil juhiseid, mida saate teha, et ***töörühmad*** [uutest](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) või [olemasolevatest](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office ' i installist eemaldada. Kui soovite, et meeskonnad oleks installitud, kuid te ei soovi, et meeskonnad hakkaks kasutaja automaatselt käivituma pärast selle installimist, lugege teemat [Microsoft teamsi automaatse käivitamise takistamine pärast installimist](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***Töörühmade desinstallimiseks*** seadmes, kus töötab Windows, lugege teemat [Microsoft teamsi desinstallimine](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Microsoft Teamsi puhastamiseks mitmest targetist või kasutajast leiate teavet teemast [Microsoft teamsi juurutuse puhastamine](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Kui kasutate ühiskasutatavaid arvuteid, kaugtöölaua teenuseid (RDS) või virtuaalse töölaua infrastruktuuri (VDI), lugege teemat [ühiskasutusse antud arvuti ja VDI keskkonnad Microsoft teamsi](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)jaoks.

Kui kasutate teenusekomplekti Office for Mac, lugege teemat [Microsoft teamsi installid Mac-arvutis](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Kui meeskonnad on installitud, [värskendatakse seda automaatselt](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) umbes iga kahe nädala järel uute funktsioonide ja kvaliteedi uuendustega. 