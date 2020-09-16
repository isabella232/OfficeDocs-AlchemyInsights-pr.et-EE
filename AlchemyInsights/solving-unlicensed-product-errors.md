---
title: Litsentsimata toote tõrgete lahendamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737949"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Tõrked "litsentsimata toote" lahendamise näpunäited

Litsentsimata toote tõrgete lahendamiseks proovige teha järgmist.

- Vaadake, kas teie tellimuse olek on aegunud.
- Veenduge, et teil on tellimus, mis lubab kliendi litsentse (nt Microsoft 365 Apps for Business või Business Premium), ja veenduge, [et kasutajal on määratud litsents](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Veenduge, et kasutaja on Office ' isse sisse loginud sama kontoga, millele on määratud litsents.
- Vaadake, kas teenusel on [teenuse seisund](https://docs.microsoft.com/office365/enterprise/view-service-health) , et näha, kas teenusega on seotud mõni teadaolev probleem.
- Kontrollige oma tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Microsoft 365 rakendusi Interneti-ühenduse jaoks. Vaadake teemat [URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Võite proovida ka järgmisi tõrkeotsingu toiminguid. 

- Avage Office ' i rakendus ja [logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mis tahes olemasolevast kasutajakontost. [Eemaldage](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) Office ' i litsents ja [määrake see uuesti](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ning seejärel [logige Office ' isse](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sisse mõjutatud kasutajakonto kaudu.
- Käivitage [aktiveerimise tõrkeotsija](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Lähtestage Office ' i aktiveerimise olek](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Office ' i võrgus parandamise](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Täiendavad tõrkeotsingu lahendused leiate järgmistest teemadest: 

- [Litsentsimata toote ja aktiveerimisega seotud tõrketeated Office’is](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Office’i aktiveerimisel kuvatakse tõrketeade: „Kahjuks ei saa teie kontoga ühendust luua. Proovige hiljem uuesti.“](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)