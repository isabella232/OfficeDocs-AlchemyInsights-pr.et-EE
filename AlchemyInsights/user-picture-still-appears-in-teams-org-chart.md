---
title: Kasutaja pilt kuvatakse endiselt Microsoft Teams organisatsiooniskeemis
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422212"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Kasutaja pilt kuvatakse endiselt Microsoft Teams organisatsiooniskeemis

Kui teie asutuse üks või mitu isikut on keelatud või eemaldatud ja tema profiilifoto kuvatakse endiselt organisatsiooniskeemil, on võimalik, et **sätte ShowInAddressLists** väärtuseks on seatud False (Väär). 

1. Avage Microsoft 365 halduskeskus > [Aktiivsed kasutajad](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) ja valige kasutaja, kellel on foto, mis endiselt kuvatakse. 
1. Valige **vahekaart Meil** ja veenduge, et suvandi **Kuva globaalses aadressiloendis väärtuseks** oleks **seatud Ei.**

Kui **sätte ShowInAddressLists** sätteks **Ei** ei tööta, kontrollige järgmist. 

- Võimalik, et kasutaja kuvatakse adressaadiloendist Exchange. Lisateavet leiate teemast [Aadressiloendite haldamine Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Kasutaja võidakse kuvada Azure Active Directory. Lisateavet leiate teemast [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 