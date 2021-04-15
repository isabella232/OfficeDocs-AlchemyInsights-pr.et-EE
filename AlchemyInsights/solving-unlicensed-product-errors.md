---
title: Litsentsimata toote tõrgete lahendamine
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
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786845"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Soovitused tõrgete "Litsentsimata toode" lahendamiseks

Litsentsimata tootega seotud tõrgete lahendamiseks proovige järgmist.

- Kontrollige, kas teie tellimuse olek on aegunud.
- Veenduge, et teil oleks tellimus, mis lubab kliendilitsentse (nt Microsoft 365 ettevõtterakendused või Business Premium) ja veenduge, et kasutajale [on määratud litsents.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Veenduge, et kasutaja logiks Office'i sisse sama kontoga, millele on määratud litsents.
- Vaadake lehel [Teenuse seisundist,](https://docs.microsoft.com/office365/enterprise/view-service-health) kas teenusega on teadaolevaid probleeme.
- Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et veenduda, et need ei blokeeri Microsoft 365 rakenduste juurdepääsu Internetile. Vt [URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Samuti võite proovida järgmisi tõrkeotsingutoiminguid. 

- Avage Office'i rakendus [ja logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mis tahes olemasolevast kasutajakontost. [Eemaldage](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [Office'i litsents](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja määrake see uuesti ning logige seejärel mõjutatud kasutajakonto abil [Office'i](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sisse.
- Käivitage [aktiveerimistõrkeotsija.](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Lähtestage Office'i aktiveerimisolekut](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Parandage Office'i võrgus.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)

Täiendavad tõrkeotsingu lahendused leiate järgmistest teemadest: 

- [Litsentsimata toote ja aktiveerimisega seotud tõrketeated Office’is](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Office’i aktiveerimisel kuvatakse tõrketeade: „Kahjuks ei saa teie kontoga ühendust luua. Proovige hiljem uuesti.“](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)