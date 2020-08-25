---
title: Saada Microsoft 365 rühmana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871760"
---
# <a name="send-as-microsoft-365-group"></a>Saada Microsoft 365 rühmana

Saate määrata käsu saada õigustega, et lubada teatud kasutajatel sõnumeid saata Microsoft 365 rühmana.  

1. Ühenduse loomine Exchange Online PowerShelliga.  

2. Käivitage järgmine käsk:  

    Add-RecipientPermission `<GroupName>` -usaldusisik `<MailboxName>` -accessrights SendAs

Lisateavet leiate teemast [liikmete saatmise lubamine või saatmine rühma nimel](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).