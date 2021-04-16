---
title: Office‘t ei saa aktiveerida
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812568"
---
# <a name="unable-to-activate-office"></a>Office‘t ei saa aktiveerida

- Kontrollige, kas teie tellimuse olek on aegunud.
- Veenduge, et teil on tellimus, mis võimaldab kliendilitsentse (nt Office 365 Business või Business Premium) ning et [kasutajal on määratud litsents](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).
- Veenduge, et kasutaja oleks Office’isse sisse logitud sama kontoga, millele on määratud litsents.
- Vaadake [Office 365 teenuste seisundi lehelt](https://docs.microsoft.com/office365/enterprise/view-service-health) järele, kas teenusega on teadaolevalt probleeme.
- Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, veendumaks, et need ei blokeeri Microsoft 365 rakenduste interneti-pääsu. Lugege teemat [Office 365 URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL-id ja IP-aadresside vahemikud").

**Näpunäide** Windowsi seadmetes saame diagnoosida ja automaatselt lahendada mitmed levinud Office'i sisselogimisprobleeme. Meie automatiseeritud tööriista kasutamiseks laadige alla ja käivitage **[Microsofti tugi- ja taasteteenuste abiline](https://aka.ms/SaRA-OfficeSignInScenario)**.

Saate kasutada järgmisi tõrkeotsingu toiminguid.

- Avage Office’i rakendus ja [logige](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) kõigist olemasolevatest kasutajakontotest välja. [Eemaldage](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) Office’i litsents ja [määrake see uuesti](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ning seejärel [logige Office’isse](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mõjutatud kasutajakontoga sisse.
- Käivitage [aktiveerimise tõrkeotsija](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Määrake uuesti Office’i aktiveerimisolek](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office’i aktiveerimisoleku lähtestamine")
- [Parandage Office võrgus](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Täiendavad tõrkeotsingu lahendused leiate järgmistest teemadest:  

- [Litsentsimata toote ja aktiveerimisega seotud tõrketeated Office’is](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Office’i aktiveerimisel kuvatakse tõrketeade: „Kahjuks ei saa teie kontoga ühendust luua. Proovige hiljem uuesti.“](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)