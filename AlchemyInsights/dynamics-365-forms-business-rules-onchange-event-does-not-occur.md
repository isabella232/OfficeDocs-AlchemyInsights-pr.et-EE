---
title: Dynamics 365 vormide ärireeglid – Ärireegel ei tulista vormi
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711487"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange sündmust ei esine, kui väli on muudetud programmiliselt

*OnChange* sündmust ei esine, kui väli on muudetud atribuudi abil programmiliselt *.* [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) meetod. Kui soovite, et *OnChange* sündmuse ohjurid töötaks pärast väärtuse määramist, peate kasutama *formContext. Data. Entity atribuut* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) meetod kood.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
