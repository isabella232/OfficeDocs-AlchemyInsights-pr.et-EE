---
title: Kasutajapilti ei kuvata Microsoft Teams organisatsiooniskeemis
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792692"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Kasutajapilti ei kuvata Microsoft Teams organisatsiooniskeemis

Kui organisatsiooniskeemis puudub ühe või mitme ettevõtte isiku profiilifoto, on võimalik, et **sätte ShowInAddressLists** väärtuseks on seatud False ( **Väär).**

1. Avage Microsoft 365 halduskeskus > [**Aktiivsed kasutajad**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)ja valige puuduva fotoga kasutaja. 
1. Valige vahekaart **Meil** ja veenduge, et suvandi **Kuva globaalses aadressiloendis väärtuseks** oleks **seatud Jah.** 

Kui **sätte ShowInAddressLists (ShowInAddressLists)** sätteks Yes (Jah) ei tööta, kontrollige järgmist. 

- Võimalik, et kasutaja on peidetud Exchange. Lisateavet leiate teemast [Aadressiloendite haldamine Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Kasutaja võib olla peidetud Azure Active Directory. Lisateavet leiate teemast [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
