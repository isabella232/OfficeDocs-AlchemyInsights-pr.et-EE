---
title: Üksik kasutaja ei näe outlooki lisandmooduleid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197833"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Üksik kasutaja ei näe outlooki lisandmooduleid

Kasutaja võib olla osa rollist, millel pole õiget parameetrit AppsForOfficeEnabled. Käivitage see cmdlet-käsk, et teada saada, kas kasutajaga on seotud õige roll:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -$false delegeerimine | Vormindus-tabel -Auto Roll,RoleAssigneeName,RoleAssigneeType

Lisateavet leiate teemast [Outlooki lisandmoodulite installimiseks ja haldamiseks administraatorite ja kasutajate määramine](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
